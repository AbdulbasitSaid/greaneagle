<template>
  <div class="">
    <ul
      class="flex items-center justify-center gap-6 text-gray-500 font-light bg-bg_gray my-4"
    >
      <li v-for="tab in tabs" :key="tab">
        <div
          :class="{
            'border-b-4 border-green-400': tab === selected,
          }"
          @click="setTab(tab)"
          class="py-4"
        >
          <div :tabs="['Description', 'Review (4)']">
            {{ tab }}
          </div>
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