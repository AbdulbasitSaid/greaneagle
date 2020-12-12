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
        <div class="flex">
          <div class="">
            <img class="w-48 h-56" src="~/assets/images/product1.png" alt="" />
          </div>
        </div>
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
</template>

<script>
export default {
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