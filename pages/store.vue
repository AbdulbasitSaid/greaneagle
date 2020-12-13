<template>
  <div>
    <div class="flex flex-col w-screen py-10 px-20">
      <!-- top -->
      <div class="flex p-6 justify-end items-center gap-10">
        <div class="flex items-center gap-4">
          <p>Show</p>
          <select name="number" id="number" class="py-2 px-4 border">
            <option value="10">10</option>
            <option value="20">20</option>
            <option value="30">30</option>
          </select>
          <p>per page</p>
        </div>
        <div class="flex items-center gap-6">
          <svg
            width="57"
            height="14"
            viewBox="0 0 57 14"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <mask
              id="mask0"
              mask-type="alpha"
              maskUnits="userSpaceOnUse"
              x="41"
              y="0"
              width="16"
              height="14"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M41 10H57V8H41V10ZM41 14H57V12H41V14ZM41 6H57V4H41V6ZM41 0V2H57V0H41Z"
                fill="white"
              />
            </mask>
            <g mask="url(#mask0)">
              <rect x="24" y="-18" width="50" height="50" fill="#D9E1E7" />
              <mask
                id="mask1"
                mask-type="alpha"
                maskUnits="userSpaceOnUse"
                x="24"
                y="-18"
                width="50"
                height="50"
              >
                <rect x="24" y="-18" width="50" height="50" fill="white" />
              </mask>
              <g mask="url(#mask1)"></g>
            </g>
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M0 7H5V1H0V7ZM0 14H5V8H0V14ZM6 14H11V8H6V14ZM12 14H17V8H12V14ZM6 7H11V1H6V7ZM12 1V7H17V1H12Z"
              fill="#2AA580"
            />
            <mask
              id="mask2"
              mask-type="alpha"
              maskUnits="userSpaceOnUse"
              x="0"
              y="1"
              width="17"
              height="13"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M0 7H5V1H0V7ZM0 14H5V8H0V14ZM6 14H11V8H6V14ZM12 14H17V8H12V14ZM6 7H11V1H6V7ZM12 1V7H17V1H12Z"
                fill="white"
              />
            </mask>
            <g mask="url(#mask2)">
              <rect x="-17" y="-17" width="50" height="50" fill="#2AA580" />
              <mask
                id="mask3"
                mask-type="alpha"
                maskUnits="userSpaceOnUse"
                x="-17"
                y="-17"
                width="50"
                height="50"
              >
                <rect x="-17" y="-17" width="50" height="50" fill="white" />
              </mask>
              <g mask="url(#mask3)"></g>
            </g>
          </svg>
          <div>Item 1 to 1,904 items</div>
        </div>
      </div>
      <!-- end top -->
      <div class="p-4 grid grid-cols-4 gap-6">
        <product-card>
          <img src="~assets/images/product1.png" />
        </product-card>
        <product-card>
          <img src="~assets/images/product2.png" />
        </product-card>
        <product-card>
          <img src="~assets/images/product3.png" />
        </product-card>
        <product-card>
          <img src="~assets/images/product4.png" />
        </product-card>
        <product-card>
          <img src="~assets/images/product5.png" />
        </product-card>
        <product-card>
          <img src="~assets/images/product6.png" />
        </product-card>
      </div>
    </div>
  </div>
</template>

<script>
import ProductCard from "../components/ProductCard.vue";
import Products from "../components/Products.vue";
export default {
  components: { Products, ProductCard },
};
</script>

<style lang="scss" scoped>
</style>