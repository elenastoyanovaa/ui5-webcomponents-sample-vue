<template>
    <ui5-date-picker></ui5-date-picker>
</template>

<script>
import "@ui5/webcomponents/dist/List";


export default {
  components: {
    TodoItem
  },
  props: ["todos"],
  methods: {
    onItemDeleted(event) {
      this.$emit('item-deleted', event);
    },
    onItemEdit(event) {
      this.$emit('item-edit', event);
    }
  }
};

</script>

<style>

</style>
