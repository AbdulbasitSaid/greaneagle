<template>
  <div v-if="isSelected" class="flex py-10">
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: { isSelected: { type: Boolean } },
};
</script>

<style lang="scss" scoped>
</style>