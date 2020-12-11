<template>
  <div>
    <div class="flex-col">
      <slider></slider>
      <features></features>
      <div class="flex-col">
        <div class="text-lg">Explore our categories</div>
      </div>
      <subscribe-now></subscribe-now>
    </div>
  </div>
</template>

<script>
import Slider from "../components/Slider.vue";
import SubscribeNow from "../components/SubscribeNow.vue";
import Tab from "../components/Tab";
import Tabs from "../components/Tabs";
export default {
  components: { SubscribeNow, Slider, Tab, Tabs },
};
</script>

<style lang="scss" scoped>
</style>