<template>
  <div class="home">
    <Hero />
    <Card v-for="(item, index) in cards" :key="index" :card="item"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Hero from '@/components/Hero.vue';
import Card from '@/components/Card.vue';

export default {
  data() {
    return {
      cards: [
        { heading: 'Awesome card 1', copy: 'Copy 1', imgSrc: 'https://loremflickr.com/g/640/480/food?lock=15' },
        { heading: 'Awesome card 2', copy: 'Copy 2', imgSrc: 'https://loremflickr.com/g/640/480/food?lock=68' },
        { heading: 'Awesome card 3', copy: 'Copy 3', imgSrc: 'https://loremflickr.com/g/640/480/food?lock=35' },
      ],
    };
  },
  name: 'home',
  components: {
    Hero,
    Card,
  },
};
</script>
