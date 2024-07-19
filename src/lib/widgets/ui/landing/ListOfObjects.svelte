
<script>
  import { ProjectCard } from '$lib/entities'
  import { projects } from '$lib/shared'
</script>

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
            <!-- {#each projects as project} -->
              <ProjectCard />
            <!-- {/each}             -->
          </div>
        </div>
      </div>
      <div class="container">
        <div class="full-div-wrap-image">
          <img src="images/originals/photo_4.jpg" loading="lazy" sizes="(max-width: 479px) 92vw, (max-width: 767px) 95vw, (max-width: 991px) 94vw, 99vw"  alt="" class="featured-image full">
        </div>
      </div>
    </section>
    