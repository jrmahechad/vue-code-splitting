<template>
  <section>
    <ImageCard v-for="(item, index) in cards" :key="index" :card="item"/>
  </section>
</template>

<script>
// @ is an alias to /src
import ImageCard from '@/components/ImageCard.vue';

export default {
  props: ['cards'],
  name: 'cards',
  components: {
    ImageCard,
  },
};
</script>
<style lang="scss" scoped>
  section {
    padding: 96px 0;
  }
</style>
