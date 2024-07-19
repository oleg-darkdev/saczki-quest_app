<script>
  const features = [
    {
      title: 'Dane historyczne',
      img: '',
      desc: 'Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
    },
    {
      title: 'Mapa interaktywna',
      img: '_2',
      desc: 'Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
    },
    {
      title: 'Chronologia przestrzeni',
      img: '_3',
      desc: 'Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
    },
  ]

</script>

<section class="section">
  <div class="container">
  <div class=" grid-col-2 studio">
    <div class="box-content section-heading studio">
      <h2 class="text1">Lorem Ipsum is simply dummy text of the printing and typesetting industry.</h2>
    </div>
  </div>
  <div class="">
    <div class="w-layout-grid grid-10">
      {#each features as {title, desc, img}}
        <div class="studio-tab">
          <div  class="wrap studio-flex">
            <div class="accordion-numbering {img}"></div>
            <h3  class="studio-tab-title">{title}</h3>
          </div>
          <p class="studio-tab-text">{desc}</p>
        </div>
      <!-- <div class="studio-tab">
        <img src="images/feature_1.png" loading="lazy" alt="Map" class="studio-featured-map-image">
      </div> -->
      {/each}
  

    </div>
  </div>
  </div>
</section>


<style>
.wrap.studio-flex {
  grid-column-gap: 15px;
  grid-row-gap: 15px;
  align-items: center;
  padding-left: 0;
  padding-right: 0;
  display: flex;
}

.grid-10 {
  grid-column-gap: 80px;
  grid-row-gap: 80px;
  grid-template-rows: auto auto;
  grid-template-columns: 1fr 1fr 1fr;
  margin-top: 60px;
  /* margin-bottom: 250px; */
}

@media screen and (max-width: 767px) {
  .container {
    padding: 20px;
  }
    .grid-10 {
    grid-column-gap: 20px;
    grid-row-gap: 20px;
    margin-top: 40px;
    /* margin-bottom: 100px; */
  }
}
@media screen and (max-width: 991px) {
  .container {
    padding: 30px;
  }
  
  .grid-10 {
    grid-column-gap: 40px;
    grid-row-gap: 40px;
    grid-template-rows: auto auto auto auto auto auto;
    grid-template-columns: 1fr;
    /* margin-top: 80px; */
  }
}

@media screen and (max-width: 479px) {
  .grid-10 {
    grid-column-gap: 40px;
    /* grid-row-gap: 65px; */
    /* margin-top: 30px; */
  }
}

.container {
  padding: 40px;
}
</style>