<template>
  <div class="">
    <ul class="flex gap-6 text-gray-500 font-light border-t border-b">
      <li v-for="tab in tabs" :key="tab">
        <div
          :class="{
            'border-t-4 border-green-400': tab === selected,
          }"
          @click="setTab(tab)"
          class="py-4"
        >
          <div
            :tabs="[
              'Mechanical Parts',
              'Electrical Parts',
              'Electronics',
              'Power supplies',
              'Systems & solutions',
            ]"
          >
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