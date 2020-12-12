<template>
  <div>
    <div class="flex-col w-48 space-y-2">
      <div class="">
        <nuxt-link to="product_detail">
          <slot></slot>
        </nuxt-link>
      </div>
      <div class="text-sm font-thin">V07106</div>
      <div class="text-sm font-thin">
        General V07106 Electric Circuit Breaker
      </div>
      <div>$105.00</div>
      <button class="border px-4 py-2 text-sm">Add to Cart</button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
</style>