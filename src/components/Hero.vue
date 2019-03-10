<template>
  <em-container>
    <em-row>
      <em-column nine>test</em-column>
      <em-column three>test</em-column>
      <em-column eight>test</em-column>
    </em-row>
  </em-container>
</template>

<script>
import EmContainer from '@/components/Container.vue';
import EmRow from '@/components/Row.vue';
import EmColumn from '@/components/Column.vue';

export default {
  name: 'hero',
  components: {
    EmContainer,
    EmRow,
    EmColumn,
  },
};
</script>

<style>
</style>
