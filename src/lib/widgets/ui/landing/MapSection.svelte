
<script>

    const mapa = [
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/1.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/2.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/3.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/4.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/5.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/6.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/7.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/8.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/9.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/10.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/11.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/12.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/13.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/14.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/15.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/16.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/17.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/18.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/19.svg',
            href: '/'
        },
        {
            title: 'Lorem Ipsum is simply dummy',
            img: '/images/numbers/20.svg',
            href: '/'
        },
    ];


    let showFull = false;
</script>

<section class="section">
    <div class="container">
        <div class="box-content section-heading">
            <h1>Mapa interaktywna</h1>
        </div>
    </div>
    <div class="container grid-col-2 ">
        <div  class="box-content">
            <h2>Lorem Ipsum is simply dummy  <br> text of the printing and typesetting industry. </h2>
            <div class="work-with-text">Lorem Ipsum is simply dummy text of the printing and typesetting industry.</div>
            <button on:click={()=> showFull = !showFull} class="work-with-link w-inline-block">
                <div class="work-with-link-text">Wyświetl pełną listę obiektów</div>
                <img src="images/64746d2efbdc4612ed8fc0e0_ArrowRight.svg" loading="lazy" alt="arrow">
            </button>
        </div>

        <div  class="box-content change-alignment fixed-width">
            <div class="work-with-link-text heading">Obiekty na mapie</div>
            {#each showFull ? mapa : mapa.slice(0,3)  as { title, img, href}}
                <a href="{href}" class="work-with-link-large w-inline-block">
                    <div class="accordion-numbering-map" style="background-image: url({img});" ></div>
                    <div class="job-text">{title}</div>
                    <img src="images/64746d2efbdc4612ed8fc0e0_ArrowRight.svg" loading="lazy"  alt="arrow">
                </a>
            {/each}
        </div>
    </div>
</section>


<style>
.accordion-numbering-map {
  width: 25px;
  height: 25px;
  background-position: 50%;
  background-repeat: no-repeat;
  background-size: auto;
  flex: none;
  justify-content: center;
  align-items: center;
  display: flex;
}

@media screen and (max-width: 767px) {
  .container {
    padding: 20px;
  }
}
@media screen and (max-width: 991px) {
  .container {
    padding: 30px;
  }
}

.container {
  padding: 40px;
  width: 100%;
}
</style>