<script>
    import Carousel from "svelte-carousel";
    const images = [
        {
            url: "https://images.pexels.com/photos/6889054/pexels-photo-6889054.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1",
            description: "image1",
        },
        {
            url: "https://images.pexels.com/photos/3074837/pexels-photo-3074837.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1",
            description: "image2",
        },
        {
            url: "https://images.pexels.com/photos/6889059/pexels-photo-6889059.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1",
            description: "image3",
        },
    ];
    let carousel; // for calling methods of the carousel instance
    const handleNextClick = () => {
        carousel.goToNext();
    };
</script>

<section id="gallery">
    <h2>User Galery</h2>
    <div class="Carousel">
        <Carousel bind:this={carousel} let:loaded>
            {#each images as src, imageIndex (src)}
                <div class="img-container">
                    {#if loaded.includes(imageIndex)}
                        <img src={src.url} alt={src.description} />
                    {/if}
                </div>
            {/each}
        </Carousel>
    </div>
</section>
