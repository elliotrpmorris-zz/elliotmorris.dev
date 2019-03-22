<template>
  <div class="grid-row">
    <slot/>
  </div>
</template>

<script>
export default {
  name: "Row"
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.grid-row {
  display: -ms-flexbox;
  width: 100%;
  display: flex;
  flex-wrap: wrap;

  &--no-wrap {
    flex-wrap: nowrap;
  }
}
</style>
