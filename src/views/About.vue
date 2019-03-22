<template>
  <div class="about">
    <em-container class="about__outer" fluid>
      <em-container class="about__inner">
        <em-row>
          <em-column class="about__content" twelve>
            <em-heading xlarge>About</em-heading>
            <em-row>
              <em-column class="about__content" six>
                <em-page-text>
                  I am a full stack developer from the UK, currently working for a tech for good agency in Leeds.
                  I love creating web apps and working with the latest tech.
                </em-page-text>
              </em-column>
              <em-column class="about__content" six>
                <em-page-text>I spend my free time working on side projects like this website!</em-page-text>
              </em-column>
            </em-row>
          </em-column>
        </em-row>
      </em-container>
    </em-container>
  </div>
</template>

<script>
import EmContainer from "@/components/Container.vue";
import EmRow from "@/components/Row.vue";
import EmColumn from "@/components/Column.vue";
import EmPageText from "@/components/PageText.vue";
import EmHeading from "@/components/Heading.vue";

export default {
  name: "about",
  components: {
    EmContainer,
    EmRow,
    EmColumn,
    EmPageText,
    EmHeading
  }
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";
.about {
  &__outer {
    background-color: $alto;
  }
  &__inner {
    background-color: $dove-grey;
  }
  &__content {
    color: $white;
    font-family: $font-primary;
    padding: map-get($map: $spaceamounts, $key: 8);

    @include tablet {
      padding: map-get($map: $spaceamounts, $key: 16);
    }
  }
}
</style>