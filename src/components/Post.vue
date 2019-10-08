<template>
  <md-card md-with-hover>
      <md-ripple>
        <md-card-header>
          <div class="md-title">{{post.heading}}</div>
        </md-card-header>

        <md-card-content>
          {{post.content}}
          </md-card-content>
      </md-ripple>
    </md-card>
</template>

<script>
export default {
  props: ['post'],
};
</script>

<style>

</style>
