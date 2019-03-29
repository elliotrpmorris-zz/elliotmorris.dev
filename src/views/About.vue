<template>
  <em-container class="about__outer" fluid>
    <em-container class="about__inner">
      <em-row>
        <em-column class="about__content" twelve>
          <em-row>
            <em-column class="about__content" tweleve>
              <em-card alto>
                <em-page-text mineShaft>
                  I am a full stack developer from the UK, currently working for a tech for good agency in Leeds.
                  I love creating web apps and working with the latest tech.
                </em-page-text>
              </em-card>
            </em-column>
          </em-row>
        </em-column>
      </em-row>
    </em-container>
  </em-container>
</template>

<script>
import EmContainer from "@/components/Container.vue";
import EmRow from "@/components/Row.vue";
import EmColumn from "@/components/Column.vue";
import EmPageText from "@/components/PageText.vue";
import EmHeading from "@/components/Heading.vue";
import EmCard from "@/components/Card.vue";

export default {
  name: "about",
  components: {
    EmContainer,
    EmRow,
    EmColumn,
    EmPageText,
    EmHeading,
    EmCard
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
    padding: space(8);

    @include bp-md {
      padding: space(16);
    }
  }
}
</style>