<template>
  <em-container>
    <em-row>
      <em-column eight>
        <em-card alto>
          <em-heading>Contact me!</em-heading>
          <em-page-text>
            Need help with a cool project?
            Email me!
            <a
              href="mailto:hello@elliotmorris.dev"
            >hello@elliotmorris.dev</a>
          </em-page-text>
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

export default {
  name: "contact",
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
