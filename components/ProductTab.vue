<template>
  <div v-if="isSelected">
    <div class="grid grid-rows-6">
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