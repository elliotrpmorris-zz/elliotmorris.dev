<template>
  <nav class="em-nav p-t-16" aria-label="Primary Navigation" role="navigation">
    <router-link class="em-nav__link p-r-16" to="/">Home 🏠</router-link>
    <router-link class="em-nav__link p-r-16" to="/about">About 📖</router-link>
    <router-link class="em-nav__link" to="/contact">Contact 🤙</router-link>
  </nav>
</template>

<script>
import EmContainer from "@/components/Container.vue";
import EmRow from "@/components/Row.vue";
import EmColumn from "@/components/Column.vue";

export default {
  name: "navigation"
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.em-nav {
  display: flex;
  justify-content: flex-end;
  &__link {
    &:after {
      content: "";
      display: block;
      width: 0;
      height: 2px;
      background: $black;
      transition: width 0.3s;
      transform: background 0.5s;
      position: relative;
      z-index: 2;
    }
    &:hover,
    &:focus {
      color: $black;
      transition: color 0.6s;
      &:after {
        width: 100%;
      }
    }
  }
}
</style>
