<template>
  <div class="bg-green-200">
    <ul>
      <li v-for="tab in tabs" :key="tab.title">
        {{ tab.title }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      selectedIndex: 0,
      tabs: [],
    };
  },
  created() {
    this.tabs = this.$children;
  },
};
</script>

<style lang="scss" scoped>
</style>