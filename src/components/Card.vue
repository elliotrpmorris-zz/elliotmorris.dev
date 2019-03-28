<template>
  <article class="em-card" :class="classes">
    <slot/>
  </article>
</template>

<script>
import EmRow from "@/components/Row.vue";
import EmColumn from "@/components/Column.vue";

export default {
  name: "card",
  components: {
    EmRow,
    EmColumn
  },

  props: {
    alto: {
      type: Boolean,
      required: false,
      default: false
    },
    round: {
      type: Boolean,
      required: false,
      default: false
    }
  },

  computed: {
    classes() {
      return {
        "em-card--alto": this.alto,
        "em-card--round": this.round
      };
    }
  }
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.em-card {
  display: flex;
  flex-direction: column;
  z-index: 1;
  position: relative;
  padding: 104px;

  &::before {
    content: " ";
    display: block;
    height: 100%;
    left: 0;
    position: absolute;
    top: 0;
    width: 100%;
    z-index: -1;
    transform: rotate(-2deg);
    box-shadow: -1px 1px 24px 0 rgba(0, 0, 0, 0.1);
  }
  &--alto {
    background-color: $alto;
    &::before {
      background-color: $alto;
    }
  }

  &--round {
    border-radius: 25%;
  }
}
</style>
