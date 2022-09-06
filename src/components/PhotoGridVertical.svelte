<script>
    import Slide from "$lib/Slide.svelte";
    export let images = [];

    function index_to_animate(index) {
        // select random animation
        let animations = [
            "animate__fadeInLeft",
            "animate__fadeInUp",
            "animate__fadeInRight",
            "animate__fadeInDown",
        ];
        return animations[Math.floor(Math.random() * animations.length)];
    }
</script>

<Slide>
    <div class="grid grid-cols-3 grid-rows-1 gap-4 lg:gap-8 p-10 justify-items-center">
        {#each images as image, index}
            <div class="h-fit animate__animated {index_to_animate(index)}">
                <img src={image.url} alt="figure-{index}" class="rounded-20" loading="lazy" />
            </div>
        {/each}
    </div>
</Slide>
