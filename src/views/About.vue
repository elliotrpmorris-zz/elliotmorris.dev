<template>
  <div class="about">
    <em-container class="about__outer" fluid>
      <em-container class="about__inner">
        <em-row>
          <em-column
            class="about__content"
            twelve
          > 
            <em-heading xlarge>About</em-heading>
            <em-text>
              I am a full stack developer from the UK, currently working for a Marketing agency in Leeds aswell as working on my own projects. 
              I work on both creating websites and software. My experience ranges from developing scripts, 
              (for example to access an API) suggesting optimization improvements, to building full blown websites with or without a CMS and hosting the site 
              I have knowledge of both linux and windows servers.
            </em-text>
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
import EmText from "@/components/Text.vue";
import EmHeading from "@/components/Heading.vue";

export default {
  name: "about",
  components: {
    EmContainer,
    EmRow,
    EmColumn,
    EmText,
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
    padding: map-get($map: $spaceamounts, $key: 32);
  }
}
</style>