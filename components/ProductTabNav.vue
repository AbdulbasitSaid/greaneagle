<template>
  <div class="w-96">
    <ul>
      <li v-for="tab in tabs" :key="tab">
        <div :class="{ 'bg-green-400': tab === selected }" @click="setTab(tab)">
          {{ tab }}
        </div>
      </li>
    </ul>
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: {
    tabs: { type: Array, required: true },
    selected: { type: String, required: true },
  },
  methods: {
    setTab(tab) {
      this.$emit("selected", tab);
    },
  },
};
</script>

<style lang="scss" scoped>
</style>