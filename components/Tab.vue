<template>
  <div v-show="isActive">
    <template slot="tabs"></template>
  </div>
</template>

<script>
export default {
  props: {
    title: { type: String, default: "Tab" },
  },
  data() {
    return { isActive: true };
  },
};
</script>

<style lang="scss" scoped>
</style>