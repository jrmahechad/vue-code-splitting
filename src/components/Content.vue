<template>
<section>
  <div class="md-layout md-gutter">
    <div class="md-layout-item md-size-40">
      <h2 class="h2">Lorem ipsum </h2>
      <h3 class="h3">Neque porro quisquam est qui dolorem ipsum quia dolor sit amet</h3>
      <p>
        Vestibulum quis luctus justo. Cras et nisl vitae velit vehicula lobortis.
        Aenean sit amet massa in ligula iaculis luctus ac quis lacus.
        Duis et tincidunt tellus. Sed eget sem ac mauris fringilla rutrum eu convallis tellus.
        Morbi id lobortis lacus, eget fringilla risus. Proin in odio id urna gravida auctor.
        Aenean non nibh et massa auctor fringilla. Praesent quis dui eu eros rhoncus pretium.
      </p>
      <md-button class="md-raised md-primary">Explore</md-button>
    </div>
    <div class="md-layout-item">
      <img src="http://lorempixel.com/1280/960/nature/8" />
    </div>
  </div>
</section>
</template>

<script>
export default {

};
</script>

<style lang="scss" scoped>
  section {
    margin: auto 10%;
  }

  .md-layout-item{
    text-align: left;
    position: relative;
  }

  .h3{
    font-size: 36px;
    line-height: 36px;
  }

  .md-raised{
    right: 0;
    position: absolute;
  }
</style>
