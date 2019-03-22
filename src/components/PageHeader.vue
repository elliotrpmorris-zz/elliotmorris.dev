<template>
  <header>
    <em-nav/>
  </header>
</template>

<script>
import EmNav from "@/components/Navigation.vue";

export default {
  name: "pageHeader",

  components: {
    EmNav
  }
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";
</style>
