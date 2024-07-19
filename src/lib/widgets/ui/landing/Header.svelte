<script>
  const navigation = [
    {
      href: '',
      title: 'Zalety'
    },
    {
      href: '',
      title: 'Mapa interaktywna'
    },
    {
      href: '',
      title: 'Obiekty artystyczne'
    },
    {
      href: '',
      title: 'Chronologia'
    },
    // {
    //   href: '',
    //   title: 'Features'
    // },
  ]

</script>



<header class="section header">
    <div class="container header grid-col-2">
      <!-- id="w-node-e0acad94-2293-5078-18d8-157ffc8138ef-ed8fc09f" -->
      <div  class="box-heading-wrap flex ">
        <div class="box-heading-content fill bg-[#6e7d33] bg-opacity-25">
          <img src="images/slogan.svg" loading="lazy" alt="SĄCZKI title" class="heading-title-svg">
        </div>
        <div class="box-heading-content bg-[#6e7d33] bg-opacity-75">
          <div class="box-content-text text">Sączki – pierwsza gdańska oczyszczalnia ścieków.</div>
          <div class="box-content-link">
            {#each navigation as {href, title}}
              <a href="{href}" class="box-content-text link type-para-intro">{title}</a>
            {/each}
          </div>
          <img src="images/64746d2efbdc4612ed8fc0bd_Arrow%202.svg" loading="lazy" alt="SĄCZKI arrow down" class="arrow">
        </div>
      </div>
      <div class="box-heading-wrap flex brand">
        <div class="heading-image"></div>
        <img src="images/logo-orange.svg" loading="lazy" alt="SĄCZKI project" class="branding">
      </div>
    </div>
  </header>


<style>

.container.header {
  background-image: url("/images/photo_4.jpg");
  background-position: 50%;
  background-repeat: no-repeat;
  background-size: cover;
}

.heading-image {
  background-image: url("/images/big-favicon.svg");
  background-position: 0 0;
  background-repeat: no-repeat;
  background-size: contain;
  flex: 1;
  padding-left: 50%;
  padding-right: 50%;
}





</style>