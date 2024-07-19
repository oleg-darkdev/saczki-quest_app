<script>
  const artistTeam = [
    {
      fullName: 'Lorem Ipsum',
      subTitle: 'Lorem Ipsum is simply',
      desc: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.',
      contact: 'loremimpsum@lorem.co.nz',
      img: 'images/artists/1.svg',
      show: false
    },
    {
      fullName: 'Lorem Ipsum',
      subTitle: 'Lorem Ipsum is simply',
      desc: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.',
      contact: 'loremimpsum@lorem.co.nz',
      img: 'images/artists/1.svg',
      show: false
    },
    {
      fullName: 'Lorem Ipsum',
      subTitle: 'Lorem Ipsum is simply',
      desc: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.',
      contact: 'loremimpsum@lorem.co.nz',
      img: 'images/artists/1.svg',
      show: false
    },
    {
      fullName: 'Lorem Ipsum',
      subTitle: 'Lorem Ipsum is simply',
      desc: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.',
      contact: 'loremimpsum@lorem.co.nz',
      img: 'images/artists/1.svg',
      show: false
    },
    {
      fullName: 'Lorem Ipsum',
      subTitle: 'Lorem Ipsum is simply',
      desc: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.',
      contact: 'loremimpsum@lorem.co.nz',
      img: 'images/artists/1.svg',
      show: false
    },
    {
      fullName: 'Lorem Ipsum',
      subTitle: 'Lorem Ipsum is simply',
      desc: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.',
      contact: 'loremimpsum@lorem.co.nz',
      img: 'images/artists/1.svg',
      show: false
    },
    {
      fullName: 'Lorem Ipsum',
      subTitle: 'Lorem Ipsum is simply',
      desc: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.',
      contact: 'loremimpsum@lorem.co.nz',
      img: 'images/artists/1.svg',
      show: false
    },
    {
      fullName: 'Lorem Ipsum',
      subTitle: 'Lorem Ipsum is simply',
      desc: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.',
      contact: 'loremimpsum@lorem.co.nz',
      img: 'images/artists/1.svg',
      show: false
    },
    {
      fullName: 'Lorem Ipsum',
      subTitle: 'Lorem Ipsum is simply',
      desc: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.',
      contact: 'loremimpsum@lorem.co.nz',
      img: 'images/artists/1.svg',
      show: false
    },
  ]

</script>

<section class="section">
  <div class="container grid-col-2">
    <div  class="box-content section-heading">
      <h1>Lista artystów</h1>
    </div>
  </div>
  <div class="container grid-col-2">
    <div class="our-team-accordion w-dyn-list">
      <div role="list" class="collection-list w-dyn-items">
        
        {#each artistTeam as {fullName, subTitle, desc, contact, img, show}}
        <div role="listitem" class="w-dyn-item">
          <div class="studio_item">
            <button on:click={()=> show = !show} class="studio_toggle w-inline-block">
              <div class="accordion-studio-grid-tab">
                <h2 class="studio_toggle-text">{fullName}</h2>
                <div class="wrap toggle-job">
                  <div class="studio_toggle-text">{subTitle}</div>
                  <div class="plus_icon_invisible">
                    <div class="plus-rotate"></div>
                    <div class="plus-fix"></div>
                  </div>
                </div>
              </div>
            </button>
            
            {#if show}
              <div class="studio_content">
                <div class="accordion-studio-grid-detail">
                  <div class="img-padding">
                    <div  class="square-img-wrap">
                      <img src="{img}" loading="lazy" alt="" class="square-img-placeholder">
                    </div>
                  </div>
                  <div class="studio-detail">
                    <div>
                      {desc}
                    </div>
                    <div>
                      <a href="{contact}" class="studio-detail-link">{contact}</a>
                    </div>
                  </div>
                </div>
              </div>
            {/if}
          </div>
        </div>
        {/each}
        
        
      </div>
    </div>
  </div>
</section>


<style>
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
  /* width: 100%; */
}

.studio-detail-link {
  color: #f29a2f;
  margin-top: 40px;
  display: block;
}

.studio-detail-link:hover {
  color: #f29a2f;
  text-decoration: underline;
}

.studio-detail {
  grid-column-gap: 40px;
  grid-row-gap: 40px;
  flex-direction: column;
  justify-content: space-between;
  display: flex;
}

.accordion-studio-grid-detail {
  grid-column-gap: 0px;
  grid-row-gap: 0px;
  grid-template-rows: auto;
  grid-template-columns: auto 47.0588%;
  grid-auto-columns: 1fr;
  padding-top: 20px;
  padding-bottom: 20px;
  display: grid;
}
  
.studio_content {
  /* height: 0; */
  display: block;
  position: relative;
  overflow: hidden;
}

.studio_content.edited {
  height: auto;
}

.accordion-studio-grid-tab {
  grid-column-gap: 0px;
  grid-row-gap: 0px;
  flex: 1;
  grid-template-rows: auto;
  grid-template-columns: auto 47.0588%;
  grid-auto-columns: 1fr;
  align-items: center;
  display: grid;
}

.our-team-accordion {
  /* margin-bottom: 190px; */
}
@media screen and (max-width: 991px) {
  .our-team-accordion {
    /* margin-bottom: 140px; */
  }
    .studio_toggle-text {
    flex: 1;
  }

  .studio-detail-link {
    display: inline;
  }

  .studio-detail {
    grid-column-gap: 30px;
    grid-row-gap: 30px;
  }

  .studio_toggle {
    height: 80px;
  }
}
@media screen and (max-width: 767px) {
  .our-team-accordion {
    /* margin-bottom: 100px; */
  }

    .studio_toggle {
    height: 54px;
  }

  .studio-detail {
    grid-column-gap: 20px;
    grid-row-gap: 20px;
    padding-right: 10px;
  }
}

.studio_item {
  width: 100%;
  border-bottom: 2px solid #6e7d33;
  margin-bottom: -2px;
  overflow: hidden;
}

.studio_item:hover {
  color: #6e7d33;
  text-decoration: none;
}


.studio_toggle {
  width: 100%;
  height: 60px;
  color: #6e7d33;
  border-top: 2px solid #6e7d33;
  border-bottom-width: 2px;
  border-bottom-color: #6e7d33;
  align-items: stretch;
  display: flex;
  position: relative;
}

.studio_toggle:hover {
  color: #6e7d33;
  text-decoration: none;
}

</style>