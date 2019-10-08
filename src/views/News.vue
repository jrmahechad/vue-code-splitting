<template>
  <div class="news">
    <Post v-for="(item, index) in posts" :key="index" :post="item" />
  </div>
</template>

<script>
import Post from '@/components/Post.vue';

const content = 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris venenatis elementum tellus, sed semper sem rhoncus at. Mauris eu posuere urna. Vestibulum fringilla, sapien eu euismod sagittis, risus ex dictum ex, ut commodo purus lectus a sem. Aliquam luctus massa lacus, pharetra volutpat tortor eleifend vel. Nam tincidunt quis justo et vulputate. Suspendisse potenti. Lorem ipsum dolor sit amet, consectetur adipiscing elit. In vel interdum ex. Suspendisse sit amet lectus aliquam, lobortis velit sit amet, commodo dui. Integer posuere nisl eget nisl imperdiet, eget porta ante fringilla. Sed eget volutpat risus. Nulla id pellentesque ante. Nullam commodo eget diam ac fringilla. Fusce consequat rhoncus metus, ac vestibulum purus. Ut vitae est vel purus posuere vehicula.';
export default {
  data() {
    return {
      posts: [
        { heading: 'Awesome news 1', content },
        { heading: 'Awesome news 2', content },
        { heading: 'Awesome news 3', content },
        { heading: 'Awesome news 4', content },
        { heading: 'Awesome news 5', content },
      ],
    };
  },
  components: {
    Post,
  },
};
</script>

<style lang="scss" scoped>
.news {
  padding: 36px 20% 0 20%;

}
.md-card {
  margin-bottom: 36px;
}
</style>
