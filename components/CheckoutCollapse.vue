<template>
  <div class="bg-white p-6 flex flex-col">
    <!-- collapser -->
    <div class="">
      <div class="flex items-center gap-4 justify-start" @click="setCollapse">
        <div
          class="rounded-full border p-2 w-10 h-10 flex items-center justify-center"
        >
          <slot name="number"> </slot>
        </div>
        <div class="text-2xl"><slot name="header"> </slot></div>
      </div>
    </div>
    <!-- end -->
    <!-- content -->
    <div class="mx-6 px-8 w-96">
      <div :class="isCollapsed ? 'hidden' : 'block'"><slot></slot></div>
    </div>
    <!-- end -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      isCollapsed: true,
    };
  },
  methods: {
    setCollapse() {
      this.isCollapsed = !this.isCollapsed;
    },
  },
};
</script>

<style lang="scss" scoped>
</style>