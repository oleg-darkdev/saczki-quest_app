<script>
    export let data;
</script>

<div role="listitem" class="w-dyn-item">
    <div class="w-layout-grid see-more-content-grid">
    <h3 id="w-node-_0c4395b5-c30d-ed42-6533-ccf53bab8194-ed8fc09f" class="see-more-text">{data.date}</h3>
    <div id="w-node-_6bce45a7-438b-2a62-ae59-9086c850c516-ed8fc09f" class="img-container rectangle-img-wrap">
        <img alt="" loading="lazy"  src="{data.img}" sizes="(max-width: 479px) 92vw, (max-width: 767px) 95vw, (max-width: 991px) 94vw, 99vw"  class="square-img-placeholder top">
        <img src="{data.img}" loading="lazy" alt="" sizes="(max-width: 479px) 92vw, (max-width: 767px) 95vw, (max-width: 991px) 94vw, 99vw"  class="square-img-placeholder lower">
    </div>
    <div id="w-node-_324dec64-756e-ca96-82aa-0b65c2ed448a-ed8fc09f" class="see-more-content">
        <div class="categories-sort w-dyn-list">
        <div role="list" class="w-dyn-items">
            <div role="listitem" class="w-dyn-item">
            <h4 class="type-para-intro see-more">{data.title}</h4>
            </div>
            <div role="listitem" class="w-dyn-item">
            <h4 class="type-para-intro see-more">{data.subTitle}</h4>
            </div>
        </div>
        </div>
        <p class="see-more-paragraph">{data.desc}</p>
    </div>
    </div>
</div>

<style>

.see-more-content-grid {
  grid-column-gap: 40px;
  grid-row-gap: 40px;
  border-bottom: 2px solid #6e7d33;
  grid-template-rows: auto;
  grid-template-columns: 1fr 1fr 2fr;
  padding-top: 20px;
  padding-bottom: 20px;
}


@media screen and (max-width: 991px) {
  .see-more-content-grid {
    grid-column-gap: 0px;
    grid-template-rows: auto 1fr;
    grid-template-columns: 1fr 1fr;
  }
}

@media screen and (max-width: 767px) {
  .see-more-content-grid {
    grid-row-gap: 20px;
  }
}
</style>