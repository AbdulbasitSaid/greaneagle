<template>
  <div v-if="isSelected">
    <div>
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