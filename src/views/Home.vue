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
        { heading: 'Awesome card 1', copy: 'Food 1', imgSrc: 'http://lorempixel.com/640/480/food/1' },
        { heading: 'Awesome card 2', copy: 'Food 2', imgSrc: 'http://lorempixel.com/640/480/food/5' },
        { heading: 'Awesome card 3', copy: 'Food 3', imgSrc: 'http://lorempixel.com/640/480/food/10' },
        { heading: 'Awesome card 4', copy: 'Food 4', imgSrc: 'http://lorempixel.com/640/480/food/8' },
      ],
      nightlifeCards: [
        { heading: 'Awesome card 1', copy: 'Nightlife 1', imgSrc: 'http://lorempixel.com/640/480/nightlife/1' },
        { heading: 'Awesome card 2', copy: 'Nightlife 2', imgSrc: 'http://lorempixel.com/640/480/nightlife/5' },
        { heading: 'Awesome card 3', copy: 'Nightlife 3', imgSrc: 'http://lorempixel.com/640/480/nightlife/10' },
        { heading: 'Awesome card 4', copy: 'Nightlife 4', imgSrc: 'http://lorempixel.com/640/480/nightlife/8' },
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
