<script>
    import Slide from '$lib/Slide.svelte'
    export let date = 'September 2021'
    export let title = 'Title'
    export let img='14.svg'
</script>

<Slide>
    <div
        class="flex flex-wrap justify-evenly items-center mx-auto max-w-22/24 pt-24"
    >
        <div
            class="lg:w-11/24 w-22/24 animate__animated animate__fadeInLeft"
        >
            <img src={img} alt="figure-1" class="rounded-20" />
        </div>
        <div class="lg:w-11/24 w-22/24 animate__animated animate__fadeInUp">
            <p
                class="font-sans font-bold text-sm text-blue-600 tracking-widest uppercase"
            >
                {date}
            </p>
            <h1
                class="font-sans font-black text-neutral-300 text-5xl text-left mt-8 tracking-tighter"
            >
                {title}
            </h1>
        </div>
    </div>
</Slide>