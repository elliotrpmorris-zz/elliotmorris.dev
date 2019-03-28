<template>
  <em-container>
    <em-row>
      <em-column six>
        <em-card alto>lorem</em-card>
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
