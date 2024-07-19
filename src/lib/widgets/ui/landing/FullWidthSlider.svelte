<script>
    import Carousel from 'svelte-carousel'
    import { browser } from '$app/environment';

    const gallery = [
        '/images/originals/photo_1.jpg',
        '/images/originals/photo_2.jpg',
        '/images/originals/photo_3.jpg',
        '/images/originals/photo_4.jpg',
    ]
</script>




<section class="section">
    <div class="container">
    <div class="box-content instagram">
        <div class="type-details"> <a href="/" target="_blank">Follow us on Instagram</a></div>
        <a href="/" target="_blank">@saczke_gdansk</a>
    </div>

    <div class="max-h-[400px] box-content instagram-embed">
       
            <div  class=" slider-img py-6 justify-between flex flex-row overflow-hidden  ">
                {#if browser}
                    <Carousel
                        autoplayDuration={0}
                        duration={5000}
                        autoplay
                        timingFunction="linear"
                        dots={false}
                        arrows={false}
                        swiping={false}
                        particlesToShow={3}
                    >
                        {#each gallery as img}
                            <img alt="" loading="lazy"  src="{img}"   class="mx-3 square-img ">
                        {/each}
                    </Carousel>
                {/if}
        </div>
    </div>
    </div>
</section>


<style>

.square-img  {
  width: 400px;
  height: 400px;
  object-fit: cover;
}

.slider-img  {
  height: 400px;
}


</style>