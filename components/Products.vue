<template>
  <div>
    <product-tab-nav
      class="flex-col"
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
        <product-card>
          <img class="h-56" src="~/assets/images/product6.png" alt="" />
        </product-card>
        <product-card>
          <img class="h-56" src="~/assets/images/product1.png" alt="" />
        </product-card>
        <product-card>
          <img class="h-56" src="~/assets/images/product3.png" alt="" />
        </product-card>
        <product-card>
          <img class="h-56" src="~/assets/images/product4.png" alt="" />
        </product-card>
      </product-tab>
      <product-tab :isSelected="selected === 'Electrical Parts'">
        <product-card>
          <img class="h-56" src="~/assets/images/product4.png" alt="" />
        </product-card>
      </product-tab>
      <product-tab :isSelected="selected === 'Electronics'">
        <product-card>
          <img class="h-56" src="~/assets/images/product3.png" alt="" />
        </product-card>
      </product-tab>

      <product-tab :isSelected="selected === 'Power supplies'">
        <product-card>
          <img class="h-56" src="~/assets/images/product2.png" alt="" />
        </product-card>
        <product-card>
          <img class="h-56" src="~/assets/images/product5.png" alt="" />
        </product-card>
        <product-card>
          <img class="h-56" src="~/assets/images/product6.png" alt="" />
        </product-card>
      </product-tab>
      <product-tab :isSelected="selected === 'Systems & solutions'">
        <product-card>
          <img class="h-56" src="~/assets/images/product3.png" alt="" />
        </product-card>
        <product-card>
          <img class="h-56" src="~/assets/images/product2.png" alt="" />
        </product-card>
        <product-card>
          <img class="h-56" src="~/assets/images/product1.png" alt="" />
        </product-card>
      </product-tab>
    </product-tab-nav>
  </div>
</template>

<script>
import ProductCard from "./ProductCard.vue";
export default {
  components: { ProductCard },
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