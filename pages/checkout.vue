<template>
  <div class="bg-checkout_bg">
    <!-- bana -->
    <div class="w-screen bg-white flex items-center justify-center gap-10">
      <!--  -->
      <div class="flex items-center gap-4">
        <div class="flex items-center gap-2">
          <svg
            width="20"
            height="20"
            viewBox="0 0 20 20"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <circle
              cx="10"
              cy="10"
              r="9.5"
              fill="#1FBE5D"
              fill-opacity="0.1"
              stroke="#1FBE5D"
            />
            <path
              opacity="0.3"
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M14.25 11.125C14.5952 11.125 14.875 10.8452 14.875 10.5C14.875 10.1548 14.5952 9.875 14.25 9.875H6.75C6.40482 9.875 6.125 10.1548 6.125 10.5C6.125 10.8452 6.40482 11.125 6.75 11.125H14.25Z"
              fill="#2AA580"
            />
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M10.9419 13.8081C11.186 14.0521 11.186 14.4479 10.9419 14.6919C10.6979 14.936 10.3021 14.936 10.0581 14.6919L6.30806 10.9419C6.07145 10.7053 6.06317 10.3243 6.28928 10.0777L9.72678 6.32767C9.96002 6.07322 10.3554 6.05603 10.6098 6.28928C10.8643 6.52252 10.8815 6.91788 10.6482 7.17233L7.61509 10.4812L10.9419 13.8081Z"
              fill="#2AA580"
            />
          </svg>

          <nuxt-link to="store" class="text-sm font-thin">
            Back to Store</nuxt-link
          >
        </div>
        <div>Checkout</div>
      </div>
      <!--  -->
      <div>
        <ul class="flex items-center gap-8 font-thin">
          <li class="border-b-4 border-primary py-4">
            <div>1. Billing Details</div>
          </li>
          <li><div>2. Shipping Details</div></li>
          <li><div>3. Delivery Method</div></li>
          <li><div>4. Payment Method</div></li>
          <li><div>5. Confirm Order</div></li>
        </ul>
      </div>
    </div>
    <!-- end -->
    <!-- main section -->
    <section class="flex items-start justify-evenly py-4 px-12">
      <!-- check out steps -->
      <div class="flex flex-col gap-6 bg-gray-300">
        <!-- billing details -->
        <checkout-collapse>
          <template v-slot:number>1</template>
          <template v-slot:header>Billing Details</template>
          <div class="flex flex-col gap-4 items-end">
            <!-- name -->
            <div class="flex items-center justify-center gap-2 mt-4 max-w-full">
              <div>
                <div>First name</div>
                <div>
                  <input
                    type="text"
                    name=""
                    id=""
                    class="rounded border w-11/12 p-2"
                  />
                </div>
              </div>
              <div>
                <div>Last name</div>
                <div>
                  <input
                    type="text"
                    name=""
                    id=""
                    class="rounded border w-11/12 p-2"
                  />
                </div>
              </div>
            </div>
            <!-- end -->
            <!-- company -->
            <div class="w-full">
              <div>Company</div>
              <div class="w-full">
                <input
                  type="text"
                  name="company"
                  id=""
                  class="w-full rounded border p-2"
                />
              </div>
            </div>
            <!-- end -->
            <!-- Address 1 -->
            <div class="w-full">
              <div>Address 1</div>
              <div class="w-full">
                <input
                  type="text"
                  name="company"
                  id=""
                  class="w-full rounded border p-2"
                />
              </div>
            </div>
            <!-- end -->
            <!-- Address 2 -->
            <div class="w-full">
              <div>Address 2</div>
              <div class="w-full">
                <input
                  type="text"
                  name="company"
                  id=""
                  class="w-full rounded border p-2"
                />
              </div>
            </div>
            <!-- end -->
            <!-- city -->
            <div
              class="flex items-center justify-between gap-2 mt-4 max-w-full"
            >
              <div>
                <div>City</div>
                <div>
                  <input
                    type="text"
                    name=""
                    id=""
                    class="rounded border w-11/12 p-2"
                  />
                </div>
              </div>
              <div>
                <div>Post code</div>
                <div>
                  <input
                    type="text"
                    name=""
                    id=""
                    class="rounded border w-11/12 p-2"
                  />
                </div>
              </div>
            </div>
            <!-- end -->
            <!-- city -->
            <div
              class="flex items-center justify-between gap-2 mt-4 max-w-full"
            >
              <div>
                <div>Country</div>
                <div>
                  <input
                    type="text"
                    name=""
                    id=""
                    class="rounded border w-11/12 p-2"
                  />
                </div>
              </div>
              <div>
                <div>Region/State</div>
                <div>
                  <input
                    type="text"
                    name=""
                    id=""
                    class="rounded border w-11/12 p-2"
                  />
                </div>
              </div>
            </div>
            <!-- end -->
          </div>
          <div class="flex justify-end py-6">
            <primary-button-rounded>Continue</primary-button-rounded>
          </div>
        </checkout-collapse>
        <!-- end -->

        <!-- Shipping Details -->
        <checkout-collapse>
          <template v-slot:number>2</template>
          <template v-slot:header>Shipping Details</template>
        </checkout-collapse>
        <!-- end -->

        <!-- Delivery Method -->
        <checkout-collapse>
          <template v-slot:number>3</template>
          <template v-slot:header>Delivery Method</template>
        </checkout-collapse>
        <!-- end -->
        <!-- Delivery Method -->
        <checkout-collapse>
          <template v-slot:number>4</template>
          <template v-slot:header>Delivery Method</template>
        </checkout-collapse>
        <!-- end -->
      </div>
      <!-- end -->
      <div></div>
    </section>
    <!-- end  -->
  </div>
</template>

<script>
import CheckoutCollapse from "../components/CheckoutCollapse.vue";
import PrimaryButtonRounded from "../components/PrimaryButtonRounded.vue";
import TextInput from "../components/TextInput.vue";
export default {
  components: { CheckoutCollapse, TextInput },
};
</script>

<style lang="scss" sc,
    PrimaryButtonRoundedoped>
</style>