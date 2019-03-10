<template>
  <div class="grid-col" :class="classes">
    <slot/>
  </div>
</template>

<script>
export default {
  name: 'column',
  props: {
    one: {
      type: Boolean,
      required: false,
      default: false,
    },
    two: {
      type: Boolean,
      required: false,
      default: false,
    },
    three: {
      type: Boolean,
      required: false,
      default: false,
    },
    four: {
      type: Boolean,
      required: false,
      default: false,
    },
    five: {
      type: Boolean,
      required: false,
      default: false,
    },
    six: {
      type: Boolean,
      required: false,
      default: false,
    },
    seven: {
      type: Boolean,
      required: false,
      default: false,
    },
    eight: {
      type: Boolean,
      required: false,
      default: false,
    },
    nine: {
      type: Boolean,
      required: false,
      default: false,
    },
    ten: {
      type: Boolean,
      required: false,
      default: false,
    },
    eleven: {
      type: Boolean,
      required: false,
      default: false,
    },
    twelve: {
      type: Boolean,
      required: false,
      default: false,
    },
  },
  computed: {
    classes() {
      return {
        'grid-col--1': this.one,
        'grid-col--2': this.two,
        'grid-col--3': this.three,
        'grid-col--4': this.four,
        'grid-col--5': this.five,
        'grid-col--6': this.six,
        'grid-col--7': this.seven,
        'grid-col--8': this.eight,
        'grid-col--9': this.nine,
        'grid-col--10': this.ten,
        'grid-col--11': this.eleven,
        'grid-col--12': this.twelve,
      };
    },
  },
};
</script>

<style lang="scss">
@import "../assets/scss/app";

.grid-col {
  box-sizing: border-box;
  background-color: green;
  border: 0.5px dashed black;
  text-align: center;
  width: 100%;
  @include tablet {
    // Column % Tablet
    &--t {
      @for $i from 1 to $total-columns {
        &--#{$i} {
          width: percentage($i/$total-columns);
        }
      }
    }
  }

  @include desktop {
    // Column % Desktop
    @for $i from 1 to $total-columns {
      &--#{$i} {
        width: percentage($i/$total-columns);
      }
    }
  }
}
</style>
