<template>
  <section class="em-hero">
    <em-container>
      <em-row>
        <em-column>
          <em-nav/>
        </em-column>
      </em-row>
      <em-row>
        <em-column twelve>
          <h1 class="em-hero__title">Yo, I'm Elliot! A Web developer from the UK.</h1>
        </em-column>
      </em-row>
    </em-container>
  </section>
</template>

<script>
import EmContainer from '@/components/Container.vue';
import EmRow from '@/components/Row.vue';
import EmColumn from '@/components/Column.vue';
import EmNav from '@/components/Navigation.vue';

export default {
  name: 'hero',
  components: {
    EmContainer,
    EmRow,
    EmColumn,
    EmNav,
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.em-hero {
  &__title {
    text-align: center;
    @include tablet {
      text-align: left;
    }
  }
}
</style>
