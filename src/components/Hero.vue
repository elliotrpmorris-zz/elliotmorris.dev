<template>
  <section class="em-hero">
    <em-container>
      <em-row>
        <em-column twelve>
          <div class="em-hero__title-wrapper">
            <em-heading xlarge class="em-hero__title">Hey, I'm Elliot! A Web developer from the UK.</em-heading>
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
import EmHeading from "@/components/Heading.vue";

export default {
  name: "hero",
  components: {
    EmContainer,
    EmRow,
    EmColumn,
    EmHeading,
  }
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.em-hero {
  &__title {
    text-align: center;
    font-size: 3.2rem;
    color: $mine-shaft;
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
