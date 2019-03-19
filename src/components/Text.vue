<template>
  <p class="text">
    <slot/>
  </p>
</template>

<script>
export default {
  name: "text"
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.text {
  font-size: $base-font-size;
  font-family: $font-primary;
  color: $white;
}
</style>
