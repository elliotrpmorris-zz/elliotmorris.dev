<template>
  <em-container>
    <em-row>
      <em-column six>
        <em-card alto>
          <em-heading large mineShaft>Asda Money</em-heading>
          <em-page-text>
            Need help with a cool project?
            Email me!
          </em-page-text>
          <em-social-bar/>
        </em-card>
      </em-column>
      <em-column six>
        <em-card alto>
          <em-heading large mineShaft>Asda Money</em-heading>
          <em-page-text>
            Need help with a cool project?
            Email me!
          </em-page-text>
          <em-social-bar/>
        </em-card>
      </em-column>
      <em-column six>
        <em-card alto>
          <em-heading large mineShaft>Asda Money</em-heading>
          <em-page-text>
            Need help with a cool project?
            Email me!
          </em-page-text>
          <em-social-bar/>
        </em-card>
      </em-column>
      <em-column six>
        <em-card alto>
          <em-heading large mineShaft>Asda Money</em-heading>
          <em-page-text>
            Need help with a cool project?
            Email me!
          </em-page-text>
          <em-social-bar/>
        </em-card>
      </em-column>
    </em-row>
  </em-container>
</template>

<script>
import EmContainer from "@/components/Container.vue";
import EmRow from "@/components/Row.vue";
import EmColumn from "@/components/Column.vue";
import EmPageText from "@/components/PageText.vue";
import EmHeading from "@/components/Heading.vue";
import EmCard from "@/components/Card.vue";
import EmSocialBar from "@/components/SocialBar.vue";

export default {
  name: "work",
  components: {
    EmContainer,
    EmRow,
    EmColumn,
    EmPageText,
    EmHeading,
    EmCard,
    EmSocialBar
  }
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";
</style>
