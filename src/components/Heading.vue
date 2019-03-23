<template>
  <h1 v-if="xlarge" class="em-heading em-heading--xl" :class="classes">
    <slot/>
  </h1>
  <h2 v-else-if="large" class="em-heading em-heading--l" :class="classes">
    <slot/>
  </h2>
  <h4 v-else-if="small" class="em-heading em-heading--s" :class="classes">
    <slot/>
  </h4>
  <h5 v-else-if="xsmall" class="em-heading em-heading--xs" :class="classes">
    <slot/>
  </h5>
  <h3 v-else class="em-heading em-heading--m" :class="classes">
    <slot/>
  </h3>
</template>

<script>
export default {
  name: "heading",

  props: {
    xlarge: {
      type: Boolean,
      required: false,
      default: false
    },
    large: {
      type: Boolean,
      required: false,
      default: false
    },
    medium: {
      type: Boolean,
      required: false,
      default: false
    },
    small: {
      type: Boolean,
      required: false,
      default: false
    },
    xsmall: {
      type: Boolean,
      required: false,
      default: false
    },
    white: {
      type: Boolean,
      required: false,
      default: false
    },
    primary: {
      type: Boolean,
      required: false,
      default: false
    },
    noMargin: {
      type: Boolean,
      required: false,
      default: false
    }
  },

  computed: {
    classes() {
      return {
        "em-heading--white": this.white,
        "em-heading--no-margin": this.noMargin,
        "em-heading--primary": this.primary,
        "em-heading--medium": this.medium
      };
    }
  }
};
</script>

<style lang="scss">
@import "../assets/scss/app";

.em-heading {
  font-family: $font-primary;
  line-height: 1;
  margin: 0.5rem 0;
  color: $white;

  &--xl {
    font-size: 2.5rem;
    font-weight: 700;
  }

  &--l {
    font-size: 2rem;
    font-weight: 700;
  }

  &--m {
    font-size: 1.5rem;
    font-weight: 600;
  }

  &--s {
    font-size: 1.25rem;
    font-weight: 600;
  }

  &--xs {
    font-size: 1rem;
    font-weight: 600;
  }

  &--no-margin {
    margin: 0;
  }

  &--white {
    color: $white;
  }
}
</style>