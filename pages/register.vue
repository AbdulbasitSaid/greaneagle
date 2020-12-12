<template>
  <div>
    <div class="flex justify-center items-center py-20">
      <div class="flex-col w-80">
        <product-list-title>Register Account</product-list-title>
        <div class="text-sm font-thin">
          If you already have an account with us
          <nuxt-link to="login" class="text-primary font-bold">
            Login</nuxt-link
          >
        </div>
        <!-- name -->
        <div class="grid grid-cols-2 text-sm font-thin">
          <div>Title</div>
          <div>First name</div>
          <div>Middle name</div>
          <div>Last name</div>
        </div>
        <!-- end -->
      </div>
    </div>
    <subscribe-now></subscribe-now>
  </div>
</template>

<script>
import ProductListTitle from "../components/ProductListTitle.vue";
export default {
  components: { ProductListTitle },
};
</script>

<style lang="scss" scoped>
</style>