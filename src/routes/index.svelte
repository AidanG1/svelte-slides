<script>
	import { images } from "$lib/images";
	import Deck from "$lib/Deck.svelte";
	import TitleSlide from "../components/TitleSlide.svelte";
	import IntroSlide from "../components/IntroSlide.svelte";
	import PhotoGrid from "../components/PhotoGrid.svelte";
	import PhotoGridVertical from "../components/PhotoGridVertical.svelte";

	let titles = {};
	let slides = [];
	let title_slides = [];

	for (let image of images) {
		let index = slides.length;
		if (titles[image.title]) {
			index = titles[image.title];
		} else {
			titles[image.title] = index;
			slides.push([]);
		}
		let slide_options = slides[index];
		if (image.title_image) {
			title_slides.push(image);
		}
		if (image.orientation == "v") {
			const is_vertical = slide_options
				.map((s) => s.vertical)
				.lastIndexOf(true);
			if (is_vertical !== -1) {
				const iv = slide_options[is_vertical];
				if (iv.images.length < 3) {
					iv.images.push(image);
				} else {
					slide_options.push({
						vertical: true,
						images: [image],
						title: false,
					});
				}
			} else {
				slide_options.push({
					vertical: true,
					images: [image],
					title: false,
				});
			}
		} else {
			const is_horizontal = slide_options
				.map((s) => s.vertical)
				.lastIndexOf(false);
			if (is_horizontal !== -1) {
				const ih = slide_options[is_horizontal];
				if (ih.images.length < 4) {
					ih.images.push(image);
				} else {
					slide_options.push({
						vertical: false,
						images: [image],
						title: false,
					});
				}
			} else {
				slide_options.push({
					vertical: false,
					images: [image],
					title: false,
				});
			}
		}
	}

	const seenTitles = new Set();

	for (let i = 0; i < slides.length; i++) {
		const slide = slides[i];
		const title_slide = title_slides.find(
			(s) => s.title === slide[0].images[0].title
		);
		if (title_slide) {
			if (!seenTitles.has(title_slide.title)) {
				slides[i] = [
					{ title: title_slide?.title, images: [title_slide] },
					...slide,
				];
				seenTitles.add(title_slide.title);
			}
		}
	}

	slides = slides;
</script>

<Deck>
	<IntroSlide />

	{#each slides as slide}
		{#each slide as slide_option}
			{#if slide_option.title}
				{@const img = slide_option.images[0]}
				<TitleSlide title={img.title} img={img.url} />
			{:else if slide_option.vertical}
				<PhotoGridVertical images={slide_option.images} />
			{:else}
				<PhotoGrid images={slide_option.images} />
			{/if}
		{/each}
	{/each}
</Deck>
