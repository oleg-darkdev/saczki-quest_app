<script>
    const project = 
    {
        title: 'Lorem Ipsum is simply',
        previewImage: 'images/64746d2efbdc4612ed8fc141_Rectangle%203.jpg',
        gallery: [
            'images/64746d2efbdc4612ed8fc141_Rectangle%203.jpg',
            'images/64746d2efbdc4612ed8fc141_Rectangle%203.jpg',
            'images/64746d2efbdc4612ed8fc141_Rectangle%203.jpg',
        ]
    }

    // export let project;
</script>

<div role="listitem" class="w-dyn-item">
    <div class="faq_item">
    <button on:click={()=> project.showProject = !project.showProject} class="faq_toggle w-inline-block">
        <div class="accordion-tab-wrap">
        <h2 class="faq_toggle-text">{project.title}</h2>
        <div class="plus-icon">
            <div class="plus-fix"></div>
            {#if !project.showProject}
                <div class="plus-rotate"></div>
            {/if}
        </div>
        </div>
        <div class="accordion-image-placeholder preview">
        <img src="{project.previewImage}" loading="lazy" alt="" sizes="(max-width: 991px) 100vw, 49vw" class="accordion-featured-image">
        </div>
        <div class="accordion-preview-mobile">
        <img src="{project.previewImage}" loading="lazy" alt="" sizes="(max-width: 479px) 82vw, (max-width: 767px) 89vw, (max-width: 991px) 85vw, 100vw" class="featured-image-mobile">
        </div>
    </button>

    {#if project.showProject}
    <div class="faq_content">
        <div class="accordion-featured-wrap">
        <div id="w-node-_0427b929-5171-2de3-d1b8-a637a4d4d370-ed8fc09f" class="accordion-featured-content">
            <div class="first-featured-content">
            <div class="first-wrap">
                <p class="type-para-intro bold first-content-size max-320px">
                    Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged.                 
                </p>
                <!-- <div class="first-featured-wrap">
                <div class="faq_small_item">
                    <a href="#" class="faq_small_toggle w-inline-block">
                    <div class="accordion-numbering"></div>
                    <div class="wrap">
                        <div class="faq_small_toggle_text">URBAN DEVELOPMENT AND INFRASTRUCTURE</div>
                        <div class="small-plus-icon">
                        <div class="small-plus-rotate"></div>
                        <div class="small-plus-fix"></div>
                        </div>
                    </div>
                    </a>
                    <div class="faq_small_content">
                    <div class="accordion-text-block max-360">Wainui Environmental provides consultancy services for developments ranging from small individual lots up to full scale catchment studies. Our services cover all stages of your project, from preliminary studies through to construction.</div>
                    </div>
                </div>              
                </div> -->
            </div>
            <div class="pattern-bar"></div>
            </div>
            <div class="last-featured-content">
            <div class="last-wrap">
                <div class="type-para-intro bold padding max-320px">
                   Lorem Ipsum is simply dummy text of the printing
                </div>
                <div class="first-featured-wrap fixed-grid">
                <div class="last-row">
                    <div class="center-flex">
                    <div class="accordion-pattern-circle-wrap">
                        <div class="accordion-pattern-inside"></div>
                    </div>
                    <div class="type-details featured-item">Lorem Ipsum is simply</div>
                    </div>
                    <div  class="center-flex">
                    <div class="accordion-pattern-circle-wrap">
                        <div class="accordion-pattern-inside"></div>
                    </div>
                    <div class="type-details featured-item">Lorem Ipsum is simply</div>
                    </div>
                    <div  class="center-flex">
                    <div class="accordion-pattern-circle-wrap">
                        <div class="accordion-pattern-inside"></div>
                    </div>
                    <div class="type-details featured-item">Lorem Ipsum is simply</div>
                    </div>
                </div>
                <!-- <div class="last-row">
                    <div id="w-node-_52722180-9d8e-c338-ff51-5b78930129fc-ed8fc09f" class="center-flex">
                    <div class="accordion-pattern-circle-wrap">
                        <div class="accordion-pattern-inside"></div>
                    </div>
                    <div class="type-details featured-item">Water Impact Assessment</div>
                    </div>
                    <div id="w-node-_52722180-9d8e-c338-ff51-5b7893012a01-ed8fc09f" class="center-flex">
                    <div class="accordion-pattern-circle-wrap">
                        <div class="accordion-pattern-inside"></div>
                    </div>
                    <div class="type-details featured-item">Three Waters Impact Assessment</div>
                    </div>
                    <div id="w-node-_52722180-9d8e-c338-ff51-5b7893012a06-ed8fc09f" class="center-flex">
                    <div class="accordion-pattern-circle-wrap">
                        <div class="accordion-pattern-inside"></div>
                    </div>
                    <div class="type-details featured-item">Flood and inundation mapping studies</div>
                    </div>
                </div>
                <div class="last-row">
                    <div id="w-node-_52722180-9d8e-c338-ff51-5b7893012a0b-ed8fc09f" class="center-flex">
                    <div class="accordion-pattern-circle-wrap">
                        <div class="accordion-pattern-inside"></div>
                    </div>
                    <div class="type-details featured-item">Design Reports</div>
                    </div>
                    <div id="w-node-_52722180-9d8e-c338-ff51-5b7893012a10-ed8fc09f" class="center-flex">
                    <div class="accordion-pattern-circle-wrap">
                        <div class="accordion-pattern-inside"></div>
                    </div>
                    <div class="type-details featured-item">River Catchment Reviews</div>
                    </div>
                    <div id="w-node-_52722180-9d8e-c338-ff51-5b7893012a15-ed8fc09f" class="center-flex">
                    <div class="accordion-pattern-circle-wrap">
                        <div class="accordion-pattern-inside"></div>
                    </div>
                    <div class="type-details featured-item">Wastewater Management Plans</div>
                    </div>
                </div>
                <div class="last-row">
                    <div id="w-node-_52722180-9d8e-c338-ff51-5b7893012a1a-ed8fc09f" class="center-flex w-condition-invisible">
                    <div class="accordion-pattern-circle-wrap">
                        <div class="accordion-pattern-inside"></div>
                    </div>
                    <div class="type-details featured-item w-dyn-bind-empty"></div>
                    </div>
                    <div id="w-node-_52722180-9d8e-c338-ff51-5b7893012a1f-ed8fc09f" class="center-flex w-condition-invisible">
                    <div class="accordion-pattern-circle-wrap">
                        <div class="accordion-pattern-inside"></div>
                    </div>
                    <div class="type-details featured-item w-dyn-bind-empty"></div>
                    </div>
                    <div id="w-node-_52722180-9d8e-c338-ff51-5b7893012a24-ed8fc09f" class="center-flex w-condition-invisible">
                    <div class="accordion-pattern-circle-wrap">
                        <div class="accordion-pattern-inside"></div>
                    </div>
                    <div class="type-details featured-item w-dyn-bind-empty"></div>
                    </div>
                </div> -->
                </div>
            </div>
            </div>
        </div>
        <div class="accordion-featured-content right">
            <div class="accordion-image-placeholder no-scrollbar">
            {#each project.gallery as img}
                <img src="{img}" loading="lazy" alt="" sizes="(max-width: 991px) 100vw, 49vw"  class="accordion-featured-image">
            {/each}
            <img src="" loading="lazy" alt="" class="accordion-featured-image w-dyn-bind-empty">
            </div>
        </div>
        </div>
    </div>
    {/if}
    </div>
</div>


<style>
.faq_content {
  background-color: #f2f2e9;
  display: block;
  position: relative;
  overflow: hidden;
}

.faq_content.edited {
  height: auto;
  overflow: visible;
}

.accordion-featured-wrap {
  grid-column-gap: 0px;
  grid-row-gap: 0px;
  grid-template-rows: auto;
  grid-template-columns: 50% 50%;
  grid-auto-columns: 1fr;
  display: grid;
}

@media screen and (max-width: 991px) {
  .accordion-featured-wrap {
    grid-template-columns: 100%;
  }
}
</style>