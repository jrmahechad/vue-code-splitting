<template>
   <md-card>
      <md-card-media>
        <img :src="card.imgSrc" alt="People">
      </md-card-media>

      <md-card-header>
        <div class="md-title">{{card.heading}}</div>
        <div class="md-subhead">{{card.copy}}</div>
      </md-card-header>
    </md-card>
</template>

<script>
export default {
  props: ['card'],
};
</script>

<style lang="scss" scoped>
  .md-card {
    display: inline-block;
    margin: 4px;
    vertical-align: top;
    width: 320px;
  }

  h1{
    font-size: 48px;
    line-height: 48px;
  }
</style>
