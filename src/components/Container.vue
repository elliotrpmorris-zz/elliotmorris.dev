<template>
  <div class="grid-container">
    <slot/>
  </div>
</template>

<script>
export default {
  name: 'container',
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.grid-container {
  max-width: $xl-screen-width;
  margin: 0 auto;

  @include tablet {
    padding: 0 $base-spacing;
  }

  &--fluid {
    margin: 0;
    max-width: 100%;
  }
}
</style>
