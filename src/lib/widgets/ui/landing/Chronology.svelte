<script>
  import { ChronologyCard } from '$lib/entities'
  import { chronology } from '$lib/shared' 

  let showChronology = false;
</script>
<!-- 
<section id="services" class="section">
      <div class="container grid-col-2 padding1">
        <div  class="box-content section-heading">
          <h1>Projekty artystyczne  <br>powiązane z SĄCZKI </h1>
        </div>
        <div  class="box-content section-description">
          <p>
            Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.          
          </p>
          <p>
            Lorem Ipsum is simply dummy text of the printing and typesetting industry.       
          </p>
        </div>
      </div>
      <div class="container">
        <div class="w-dyn-list">
          <div role="list" class="w-dyn-items">

          </div>
        </div>
      </div>
      <div class="container">
        <div class="full-div-wrap-image">
          <img src="images/originals/photo_4.jpg" loading="lazy" sizes="(max-width: 479px) 92vw, (max-width: 767px) 95vw, (max-width: 991px) 94vw, 99vw"  alt="" class="featured-image full">
        </div>
      </div>
    </section>

     -->
<section class="section">
      <div class="container">
        <!-- style="height:110px" -->
        <div  class="accordion w-dropdown">
          <div class="accordion-toggle w-dropdown-toggle">
        <button on:click={()=> showChronology = !showChronology} class="faq_toggle w-inline-block">
        <div class="accordion-tab-wrap ">
        <h2 class="faq_toggle-text">Chronologia</h2>
        <div class="plus-icon">
            <div class="plus-fix"></div>
            {#if !showChronology}
                <div class="plus-rotate"></div>
            {/if}
        </div>
        </div>
    </button>

            <!-- <h2 style="color:rgb(110,125,51)" class="accordion-tab-title">Chronologia


                      <div class="plus-icon">
            <div class="plus-fix"></div>
            {#if !showChronology}
                <div class="plus-rotate"></div>
            {/if}
        </div>
            </h2> -->
            <!-- <div class="plus-icon">
              <div style="background-color:rgb(110,125,51);-webkit-transform:translate3d(0, 0, 0) scale3d(1, 1, 1) rotateX(0) rotateY(0) rotateZ(0deg) skew(0, 0);-moz-transform:translate3d(0, 0, 0) scale3d(1, 1, 1) rotateX(0) rotateY(0) rotateZ(0deg) skew(0, 0);-ms-transform:translate3d(0, 0, 0) scale3d(1, 1, 1) rotateX(0) rotateY(0) rotateZ(0deg) skew(0, 0);transform:translate3d(0, 0, 0) scale3d(1, 1, 1) rotateX(0) rotateY(0) rotateZ(0deg) skew(0, 0)" class="plus-rotate"></div>
              <div style="background-color:rgb(110,125,51)" class="plus-fix"></div>
            </div> -->
          </div>
          
          <nav class="accordion-content see-more w-dropdown-list">
            <div class="projects-collection w-dyn-list">
              <div role="list" class="w-dyn-items">
                {#each showChronology ? chronology : chronology.slice(0, 1) as data}
                    <ChronologyCard {data} />
                {/each}
              </div>
            </div>
          </nav>
        </div>
      </div>
    </section>



<style>
  
.w-dropdown-list {
  min-width: 100%;
  background: #ddd;
  /* display: none; */
  position: absolute;
}
@media screen and (max-width: 991px) {

  .img-container {
  grid-area: span 1 / span 1 / span 1 / span 1;
}
}

  .img-container {
    grid-area: span 2 / span 1 / span 2 / span 1;
  }



.w-dropdown-list.w--open {
  display: block;
}

.accordion-content {
  background-color: #f2f2e9;
  display: block;
  position: static;
}

.accordion-content.see-more {
  border-bottom-style: none;
}


.see-more-content {
  padding-left: 80px;
  padding-right: 32.8125%;
}


.type-para-intro.see-more {
  margin-top: 0;
  margin-bottom: 0;
  font-size: 14px;
}

.see-more-text {
  text-transform: uppercase;
}

.see-more-paragraph {
  max-width: 360px;
}


@media screen and (max-width: 991px) {
  .see-more-content {
    padding-left: 0;
    padding-right: 25%;
  }
  .type-para-intro.see-more {
    font-size: 12px;
  }

  .see-more-text {
    margin-right: 12.5%;
  }

  .see-more-paragraph {
    display: none;
  }

}

@media screen and (max-width: 767px) {
  .type-para-intro.see-more {
    font-size: 8.8px;
  }

}


</style>