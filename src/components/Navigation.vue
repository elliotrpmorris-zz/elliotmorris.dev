<template>
  <nav class="em-nav" aria-label="Primary Navigation" role="navigation">
    <router-link class="em-nav__link p-r-16" to="/">Home</router-link>
    <router-link class="em-nav__link" to="/about">About</router-link>
  </nav>
</template>

<script>
export default {
  name: 'navigation',
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.em-nav {
  text-align: right;
}
</style>
