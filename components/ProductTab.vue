<template>
  <div v-if="isSelected">
    <div class="grid grid-cols-4 gap-6 py-20">
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  props: { isSelected: { type: Boolean } },
};
</script>

<style lang="scss" scoped>
</style>