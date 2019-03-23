<template>
  <article class="em-card">
    <em-heading medium>My work</em-heading>
    <em-page-text>
      <slot/>
    </em-page-text>
  </article>
</template>

<script>
import EmRow from "@/components/Row.vue";
import EmColumn from "@/components/Column.vue";
import EmHeading from "@/components/Heading.vue";
import EmPageText from "@/components/PageText.vue";

export default {
  name: "card",
  components: {
    EmRow,
    EmColumn,
    EmHeading,
    EmPageText
  }
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.em-card {
  display: flex;
  flex-direction: column;
}
</style>
