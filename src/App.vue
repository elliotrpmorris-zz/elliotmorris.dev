<template>
  <main id="app">
    <em-nav/>
    <router-view/>
  </main>
</template>

<script>
import EmNav from '@/components/Navigation.vue';

export default {
  components: {
    EmNav,
  },
};
</script>

<style lang="scss">
@import "../src/assets/scss/app";
</style>
