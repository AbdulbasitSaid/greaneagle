<template>
  <div class="">
    <!-- collapse -->
    <div class="w-full p-2">
      <div
        class="collapsible flex items-center justify-between py-2 border-b"
        ref="collapse"
        @click="collapseItem"
      >
        <div>
          <slot name="heading"></slot>
        </div>
        <div>+</div>
      </div>
      <div
        class="content overflow-hidden"
        :class="collapsed ? ' block' : 'hidden'"
      >
        <slot></slot>
      </div>
    </div>
    <!-- end  -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      collapsed: false,
    };
  },
  methods: {
    collapseItem() {
      this.collapsed = !this.collapsed;
    },
  },
};
</script>

<style lang="scss" scoped>
</style>