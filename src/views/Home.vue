<template>
  <div class="home">
    <Hero />
    <Cards :cards="foodCards"/>
    <Content/>
    <Cards :cards="nightlifeCards"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Hero from '@/components/Hero.vue';
import Cards from '@/components/Cards.vue';
import Content from '@/components/Content.vue';

export default {
  data() {
    return {
      foodCards: [
        { heading: 'Awesome card 1', copy: 'Food 1', imgSrc: 'food1' },
        { heading: 'Awesome card 2', copy: 'Food 2', imgSrc: 'food2' },
        { heading: 'Awesome card 3', copy: 'Food 3', imgSrc: 'food3' },
        { heading: 'Awesome card 4', copy: 'Food 4', imgSrc: 'food4' },
      ],
      nightlifeCards: [
        { heading: 'Awesome card 1', copy: 'Nightlife 1', imgSrc: 'social1' },
        { heading: 'Awesome card 2', copy: 'Nightlife 2', imgSrc: 'social2' },
        { heading: 'Awesome card 3', copy: 'Nightlife 3', imgSrc: 'social3' },
        { heading: 'Awesome card 4', copy: 'Nightlife 4', imgSrc: 'social4' },
      ],
    };
  },
  name: 'home',
  components: {
    Hero,
    Cards,
    Content,
  },
};
</script>
