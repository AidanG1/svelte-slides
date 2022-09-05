<script>
	import Slide from "$lib/Slide.svelte";
	import Deck from "$lib/Deck.svelte";
	import Vizzu from "$lib/Vizzu.svelte";
	import TitleSlide from "../components/TitleSlide.svelte";
	import IntroSlide from "../components/IntroSlide.svelte";
	import PhotoGrid from "../components/PhotoGrid.svelte";
	import PhotoGridVertical from "../components/PhotoGridVertical.svelte";
	import { data } from "https://lib.vizzuhq.com/test/integration/test_data/infinite_data.js?client";
</script>

<Deck>
	<IntroSlide />

	<TitleSlide
		date="December 2021"
		title="Filoli Gardens"
		img="/Filoli/IMG_5566.jpg"
	/>

	<PhotoGrid
		images={[
			"/Filoli/IMG_5504.jpg",
			"/Filoli/IMG_5507.jpg",
			"/Filoli/IMG_5528.jpg",
			"/Filoli/IMG_5625.jpg",
		]}
	/>

	<TitleSlide
		date="December 2021"
		title="Death Valley"
		img="/DV/IMG_5782.jpg"
	/>

	<PhotoGrid
		images={[
			"/DV/IMG_5689.jpg",
			"/DV/IMG_5796.jpg",
			"/DV/IMG_5913.jpg",
			"/DV/IMG_5921.jpg",
		]}
	/>

	<PhotoGridVertical
		images={["/DV/IMG_5877.jpg", "/DV/IMG_5891.jpg", "/DV/IMG_5924.jpg"]}
	/>

	<PhotoGridVertical
		images={["/DV/IMG_5930.jpg", "/DV/IMG_5932.jpg", "/DV/IMG_5936.jpg"]}
	/>

	<PhotoGrid
		images={[
			"/DV/IMG_5935.jpg",
			"/DV/IMG_5809.jpg",
			"/DV/IMG_5940.jpg",
			"/DV/IMG_5946.jpg",
		]}
	/>

	<PhotoGrid
		images={[
			"/DV/IMG_5952.jpg",
			"/DV/IMG_5985.jpg",
			"/DV/IMG_6007.jpg",
			"/DV/IMG_6009.jpg",
		]}
	/>

	<PhotoGridVertical
		images={["/DV/IMG_5923.jpg", "/DV/IMG_6002.jpg", "/DV/IMG_6048.jpg"]}
	/>

	<PhotoGrid
		images={[
			"/DV/IMG_6131.jpg",
			"/DV/IMG_6141.jpg",
			"/DV/IMG_6160.jpg",
			"/DV/IMG_6121.jpg",
		]}
	/>

	<PhotoGridVertical
		images={["/DV/IMG_6134.jpg", "/DV/IMG_6079.jpg", "/DV/IMG_6138.jpg"]}
	/>

	<PhotoGridVertical
		images={["/DV/IMG_6152.jpg", "/DV/IMG_6161.jpg", "/DV/IMG_6155.jpg"]}
	/>

	<TitleSlide date="December 2021" title="Dunes" img="/Dunes/IMG_6374.jpg" />

	<PhotoGrid
		images={[
			"/Dunes/IMG_6180.jpg",
			"/Dunes/IMG_6207.jpg",
			"/Dunes/IMG_6235.jpg",
			"/Dunes/IMG_6261.jpg",
		]}
	/>

	<PhotoGridVertical
		images={[
			"/Dunes/IMG_6206.jpg",
			"/Dunes/IMG_6271.jpg",
			"/Dunes/IMG_6353.jpg",
		]}
	/>

	<PhotoGrid
		images={[
			"/Dunes/IMG_6280.jpg",
			"/Dunes/IMG_6310.jpg",
			"/Dunes/IMG_6333.jpg",
			"/Dunes/IMG_6374.jpg",
		]}
	/>

	<TitleSlide
		date="December 2021"
		title="Joshua Tree 1"
		img="/JT1/IMG_6695.jpg"
	/>

	<PhotoGrid
		images={[
			"/JT1/IMG_6398.jpg",
			"/JT1/IMG_6406.jpg",
			"/JT1/IMG_6495.jpg",
			"/JT1/IMG_6500.jpg",
		]}
	/>

	<PhotoGridVertical
		images={["/JT1/IMG_6422.jpg", "/JT1/IMG_6445.jpg", "/JT1/IMG_6543.jpg"]}
	/>

	<PhotoGrid
		images={[
			"/JT1/IMG_6507.jpg",
			"/JT1/IMG_6561.jpg",
			"/JT1/IMG_6575.jpg",
			"/JT1/IMG_6587.jpg",
		]}
	/>

	<PhotoGridVertical
		images={["/JT1/IMG_6581.jpg", "/JT1/IMG_6590.jpg", "/JT1/IMG_6651.jpg"]}
	/>

	<PhotoGrid
		images={[
			"/JT1/IMG_6592.jpg",
			"/JT1/IMG_6599.jpg",
			"/JT1/IMG_6634.jpg",
			"/JT1/IMG_6660.jpg",
		]}
	/>

	<PhotoGrid
		images={[
			"/JT1/IMG_6614.jpg",
			"/JT1/IMG_6694.jpg",
			"/JT1/IMG_6647.jpg",
			"/JT1/IMG_6667.jpg",
		]}
	/>

	<TitleSlide
		date="December 2021"
		title="Joshua Tree 2"
		img="/JT2/IMG_6712.jpg"
	/>

	<PhotoGrid
		images={[
			"/JT2/IMG_6712.jpg",
			"/JT2/IMG_6728.jpg",
			"/JT2/IMG_6740.jpg",
			"/JT2/IMG_6761.jpg",
		]}
	/>

	<PhotoGrid
		images={[
			"/JT2/IMG_6776.jpg",
			"/JT2/IMG_6778.jpg",
			"/JT2/IMG_6784.jpg",
			"/JT2/IMG_6790.jpg",
		]}
	/>

	<TitleSlide
		date="December 2021"
		title="Joshua Tree 3 & 4"
		img="/JT3/IMG_6817.jpg"
	/>

	<PhotoGrid
		images={[
			"/JT3/IMG_6803.jpg",
			"/JT3/IMG_6810.jpg",
			"/JT3/IMG_6819.jpg",
			"/JT3/IMG_6846.jpg",
		]}
	/>

	<PhotoGridVertical
		images={["/JT3/IMG_6820.jpg", "/JT3/IMG_6836.jpg", "/JT3/IMG_6843.jpg"]}
	/>

	<PhotoGridVertical
		images={["/JT4/IMG_6862.jpg", "/JT4/IMG_6870.jpg", "/JT4/IMG_6890.jpg"]}
	/>

	<TitleSlide
		date="December 2021"
		title="Palm Springs"
		img="/PS/IMG_6949.jpg"
	/>

	<PhotoGrid
		images={[
			"/PS/IMG_6932.jpg",
			"/PS/IMG_6944.jpg",
			"/PS/IMG_6953.jpg",
			"/PS/IMG_6963.jpg",
		]}
	/>

	<PhotoGrid
		images={[
			"/PS/IMG_6972.jpg",
			"/PS/IMG_6989.jpg",
			"/PS/IMG_7006.jpg",
			"/PS/IMG_shoe.jpg",
		]}
	/>

	<PhotoGrid
		images={[
			"/PS/IMG_7051.jpg",
			"/PS/IMG_7067.jpg",
			"/PS/IMG_7080.jpg",
			"/PS/IMG_7184.jpg",
		]}
	/>

	<PhotoGrid
		images={[
			"/PS/IMG_7121.jpg",
			"/PS/IMG_7124.jpg",
			"/PS/IMG_7128.jpg",
			"/PS/IMG_7134.jpg",
		]}
	/>

	<PhotoGrid
		images={[
			"/PS/IMG_7139.jpg",
			"/PS/IMG_7148.jpg",
			"/PS/IMG_7171.jpg",
			"/PS/IMG_7181.jpg",
		]}
	/>

	<PhotoGridVertical images={["/SM/1.jpg", "/SM/3.jpg", "/SM/2.jpg"]} />

	<TitleSlide
		date="January-February 2021"
		title="Random School Pictures"
		img="/RSP/IMG_8027.jpg"
	/>

	<PhotoGrid
		images={[
			"/RSP/Datathon1.jpg",
			"/RSP/Datathon2.jpg",
			"/RSP/Rock1.jpg",
			"/RSP/Rock2.jpg",
		]}
	/>

	<PhotoGrid
		images={[
			"/RSP/Hawk.jpg",
			"/RSP/IMG_7898.jpg",
			"/RSP/IMG_7903.jpg",
			"/RSP/IMG_7278.jpg",
		]}
	/>

	<PhotoGridVertical
		images={["/RSP/IMG_7502.jpg", "/RSP/IMG_7602.jpg", "/RSP/IMG_7715.jpg"]}
	/>

	<PhotoGridVertical
		images={["/RSP/IMG_7972.jpg", "/RSP/IMG_7950.jpg", "/RSP/IMG_7984.jpg"]}
	/>

	<PhotoGrid
		images={[
			"/RSP/IMG_8007.jpg",
			"/RSP/IMG_8027.jpg",
			"/RSP/Reflection1.jpg",
			"/RSP/Reflection2.jpg",
		]}
	/>
</Deck>
