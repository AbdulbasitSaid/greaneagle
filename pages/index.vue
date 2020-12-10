<template>
  <div>
    <div class="flex-col">
      <slider></slider>
      <subscribe-now></subscribe-now>
    </div>
  </div>
</template>

<script>
import Slider from "../components/Slider.vue";
import SubscribeNow from "../components/SubscribeNow.vue";
export default {
  components: { SubscribeNow, Slider },
};
</script>

<style lang="scss" scoped>
</style>