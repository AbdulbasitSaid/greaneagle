<template>
  <div class="flex flex-col py-6 px-12">
    <div class="flex items-center justify-between">
      <div class="text-lg">
        Your shopping list
        <div class="text-sm font-thin">
          You have 3 items in your shopping cart
        </div>
      </div>
      <nuxt-link to="store" class="border py-2 px-4"
        >Continue Shopping</nuxt-link
      >
    </div>
    <!-- cart table -->
    <table>
      <!-- heading  -->
      <tr class="font-bold py-2 h-24 border-b">
        <td class="w-48"></td>
        <td class="w-48">Product Name</td>
        <td class="w-48">Model</td>
        <td class="w-48">Quantity</td>
        <td class="w-48">Unit Price ($)</td>
        <td class="w-48">Total ($)</td>
        <td></td>
      </tr>
      <!-- end -->
      <!-- cart item -->
      <tr class="h-28 border-b">
        <td class="">
          <img src="~/assets/images/product1.png" alt="" class="w-24" />
        </td>
        <td>31002060011</td>
        <td>31002060011</td>
        <td><increase></increase></td>
        <td>3500.00</td>
        <td>3500.00</td>
        <td><cancel></cancel></td>
      </tr>
      <!-- end  -->
      <!-- cart item -->
      <tr class="h-28 border-b">
        <td class="">
          <img src="~/assets/images/product6.png" alt="" class="w-24" />
        </td>
        <td>31002060011</td>
        <td>31002060011</td>
        <td><increase></increase></td>
        <td>3500.00</td>
        <td>3500.00</td>
        <td><cancel></cancel></td>
      </tr>
      <!-- end  -->
      <!-- cart item -->
      <tr class="h-28 border-b">
        <td class="">
          <img src="~/assets/images/product5.png" alt="" class="w-24" />
        </td>
        <td>31002060011</td>
        <td>31002060011</td>
        <td><increase></increase></td>
        <td>3500.00</td>
        <td>3500.00</td>
        <td><cancel></cancel></td>
      </tr>
      <!-- end  -->
    </table>
    <!-- end -->

    <div class="flex justify-end p-4">
      <!-- collapse -->
      <div class="w-2/5">
        <collabsable>
          <template v-slot:heading> Use coupon code </template>
          <div class="py-4 flex flex-col gap-2">
            <input
              type="text"
              name=""
              id=""
              class="rounded p-2 border w-full"
              placeholder="add coupon"
            />
            <div>
              <input
                type="button"
                value="Apply coupon"
                class="rounded text-white py-2 px-6 bg-bg_footer"
              />
            </div>
          </div>
        </collabsable>
        <collabsable>
          <template v-slot:heading> Estimate shipping & taxes </template>
          <div class="flex flex-col gap-4 py-4">
            <!-- country -->
            <div class="text-sm">
              <div class="flex flex-col">
                Country
                <input
                  type="text"
                  name=""
                  id=""
                  class="border p-2 rounded w-full block"
                  placeholder="Nigeria"
                />
              </div>
            </div>
            <!-- end -->
            <div class="flex">
              <div>
                State
                <input
                  type="text"
                  name=""
                  id=""
                  class="border p-2 rounded"
                  placeholder="Lagos"
                />
              </div>
              <div>
                Post code
                <input
                  type="text"
                  name=""
                  id=""
                  class="border p-2 rounded"
                  placeholder="900211"
                />
              </div>
            </div>
            <div>
              <input
                type="button"
                value="Get quotes "
                class="rounded text-white py-2 px-6 bg-bg_footer"
              />
            </div>
          </div>
        </collabsable>
        <collabsable>
          <template v-slot:heading> Use gift certificate </template>
          <div class="py-4 flex flex-col gap-2">
            <input
              type="text"
              name=""
              id=""
              class="rounded p-2 border w-full"
              placeholder="Enter gift code here"
            />
            <div>
              <input
                type="button"
                value="Apply "
                class="rounded text-white py-2 px-6 bg-bg_footer"
              />
            </div>
          </div>
        </collabsable>
        <div class="w-full p-2">
          <div
            class="collapsible flex items-center justify-between py-2 border-b"
            ref="collapse"
          >
            <div>Sub-Total</div>
            <div>15,050.00</div>
          </div>
          <div
            class="content overflow-hidden"
            :class="collapsed ? ' block' : 'hidden'"
          >
            <slot></slot>
          </div>
        </div>
        <div class="w-full p-2">
          <div
            class="collapsible flex items-center justify-between py-2 border-b"
            ref="collapse"
          >
            <div>Total</div>
            <div>15,050.00</div>
          </div>
          <div
            class="content overflow-hidden"
            :class="collapsed ? ' block' : 'hidden'"
          >
            <slot></slot>
          </div>
        </div>

        <div class="flex justify-end py-10">
          <nuxt-link
            to="check_out"
            class="rounded bg-primary text-white py-2 px-4"
            >Checkout as guest</nuxt-link
          >
        </div>
        <div class="flex justify-end py-10 items-center gap-2">
          <div>Already registered?</div>
          <nuxt-link to="login" class="text-golden"
            >Login to continue</nuxt-link
          >
        </div>
      </div>
      <!-- end  -->
    </div>
  </div>
</template>

<script>
import Cancel from "../components/Cancel.vue";
import Collabsable from "../components/Collabsable.vue";
import Increase from "../components/Increase.vue";
export default {
  components: { Increase, Cancel, Collabsable },
  data() {
    return {};
  },
  methods: {},
};
</script>

<style scoped>
.content {
  padding: 0 18px;
  display: none;
  overflow: hidden;
  background-color: #f1f1f1;
}
</style>