<template>
  <div class="grid-row">
    <slot/>
  </div>
</template>

<script>
export default {
  name: 'Row',
};
</script>

<style lang="scss">
@import "../assets/scss/app";

.grid-row {
  display: -ms-flexbox;
  -ms-flex-wrap: wrap;
  display: flex;
  flex-wrap: wrap;
  margin: 0 -1rem;
  // Remove Wrap
  &--no-wrap {
    flex-wrap: nowrap;
  }
}
</style>
