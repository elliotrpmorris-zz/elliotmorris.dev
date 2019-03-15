<template>
  <section class="em-hero">
    <em-container>
      <em-row>
        <em-column twelve>
          <div class="em-hero__title-wrapper m-t-16">
            <h2 class="em-hero__title">I currently focus on front end development</h2>
          </div>
        </em-column>
      </em-row>
    </em-container>
  </section>
</template>

<script>
import EmContainer from "@/components/Container.vue";
import EmRow from "@/components/Row.vue";
import EmColumn from "@/components/Column.vue";

export default {
  name: "contentBlock",
  components: {
    EmContainer,
    EmRow,
    EmColumn
  }
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.em-hero {
  &__title {
    text-align: center;
    font-size: 3rem;
    @include tablet {
      text-align: left;
      font-size: 4rem;
    }
  }
  &__title-wrapper {
    background-color: $alto;
    padding: $spacing-l $spacing-xl;
  }
}
</style>
