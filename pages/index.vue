<template>
  <div>
    <div class="flex-col">
      <slider></slider>
      <features></features>
      <div class="flex-col">
        <div class="text-lg">Explore our categories</div>
        <product-tab-nav
          :tabs="[
            'Mechanical Parts',
            'Electrical Parts',
            'Electronics',
            'Power supplies',
            'Systems & solutions',
          ]"
          :selected="selected"
          @selected="setSelected"
        >
          <product-tab :isSelected="selected === 'Mechanical Parts'">
            Mechanical Parts selected
          </product-tab>
          <product-tab :isSelected="selected === 'Electrical Parts'">
            Electrical Parts selected
          </product-tab>
          <product-tab :isSelected="selected === 'Electronics'">
            Electronics selected
          </product-tab>
          <product-tab :isSelected="selected === 'Power supplies'">
            Power Parts selected
          </product-tab>
          <product-tab :isSelected="selected === 'Systems & solutions'">
            Systems & solutions selected
          </product-tab>
        </product-tab-nav>
      </div>
      <subscribe-now></subscribe-now>
    </div>
  </div>
</template>

<script>
import ProductTab from "../components/ProductTab.vue";
import ProductTabNav from "../components/ProductTabNav.vue";
import Slider from "../components/Slider.vue";
import SubscribeNow from "../components/SubscribeNow.vue";

export default {
  components: { SubscribeNow, Slider, ProductTabNav, ProductTab },
  data() {
    return { selected: "Mechanical Parts" };
  },
  methods: {
    setSelected(tab) {
      this.selected = tab;
    },
  },
};
</script>

<style lang="scss" scoped>
</style>