<template>
  <div>
    <div class="flex-col">
      <slider></slider>
      <features></features>
      <div class="p-12">
        <div class="flex-col">
          <product-list-title>Explore our categories</product-list-title>
          <products></products>
        </div>
      </div>
      <subscribe-now></subscribe-now>
    </div>
  </div>
</template>

<script>
import ProductListTitle from "../components/ProductListTitle.vue";
import Products from "../components/Products.vue";
import Slider from "../components/Slider.vue";
import SubscribeNow from "../components/SubscribeNow.vue";

export default {
  components: { SubscribeNow, Slider, Products, ProductListTitle },
};
</script>

<style lang="scss" scoped>
</style>