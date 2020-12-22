<template>
  <div>
    <main>
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
                <div
                  class="flex items-center justify-center gap-2 mt-4 max-w-full"
                >
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
              <div class="space-y-2">
                <!--  -->
                <div class="flex flex-col items-center w-full gap-4">
                  <!-- radio -->
                  <div class="flex items-center gap-4">
                    <input
                      type="radio"
                      id="existing"
                      name="existing"
                      value="existing"
                      class=""
                    />
                    <label for="existing"
                      >I want to use an existing address</label
                    ><br />
                  </div>
                  <!-- end -->
                  <textarea
                    name=""
                    id=""
                    cols="30"
                    rows="6"
                    class="border rounded"
                  ></textarea>
                </div>
                <!--  -->
                <!-- radio -->
                <div class="flex items-center gap-4">
                  <input
                    type="radio"
                    id="existing"
                    name="existing"
                    value="existing"
                    class=""
                  />
                  <label for="existing">I want to use my billing address</label
                  ><br />
                </div>
                <!-- end -->
                <!-- radio -->
                <div class="flex items-center gap-4">
                  <input
                    type="radio"
                    id="existing"
                    name="existing"
                    value="existing"
                    class=""
                  />
                  <label for="existing">I want to use a new address</label
                  ><br />
                </div>
                <!-- end -->
              </div>
              <div class="flex justify-end py-4">
                <primary-button-rounded>Continue</primary-button-rounded>
              </div>
            </checkout-collapse>
            <!-- end -->

            <!-- Delivery Method -->
            <checkout-collapse>
              <template v-slot:number>3</template>
              <template v-slot:header>Delivery Method</template>
              <div>
                <!-- radio -->
                <div class="flex items-center gap-4">
                  <input
                    type="radio"
                    id="existing"
                    name="existing"
                    value="existing"
                    class=""
                  />
                  <label for="existing"
                    >UPS Worldwide Express Plus -
                    <span class="text-golden">$442.57</span></label
                  ><br />
                </div>
                <!-- end -->
                <!-- radio -->
                <div class="flex items-center gap-4">
                  <input
                    type="radio"
                    id="existing"
                    name="existing"
                    value="existing"
                    class=""
                  />
                  <label for="existing"
                    >UPS Saver - <span class="text-golden">$393.71</span></label
                  ><br />
                </div>
                <!-- end -->
                <!-- radio -->
                <div class="flex items-center gap-4">
                  <input
                    type="radio"
                    id="existing"
                    name="existing"
                    value="existing"
                    class=""
                  />
                  <label for="existing"
                    >UPS Worldwide Express
                    <span class="text-golden">- $401.57</span></label
                  ><br />
                </div>
                <!-- end -->
              </div>
            </checkout-collapse>
            <!-- end -->
            <!-- Delivery Method -->
            <checkout-collapse>
              <template v-slot:number>4</template>
              <template v-slot:header>Payment Method</template>
              <div>
                <div class="flex items-center gap-4">
                  <input
                    type="radio"
                    id="existing"
                    name="existing"
                    value="existing"
                    class=""
                  />
                  <label for="existing">PayPal Express Checkout</label><br />
                </div>
                <!--  -->
                <div class="flex items-center gap-4">
                  <input
                    type="radio"
                    id="existing"
                    name="existing"
                    value="existing"
                    class=""
                  />
                  <label for="existing">Credit or Debit Cardt</label><br />
                </div>
                <!-- end -->
              </div>
              <div class="flex items-center gap-4">
                <input type="checkbox" name="" id="" />I have read and agree to
                the Terms & Conditions
              </div>

              <div>
                <textarea
                  name=""
                  id=""
                  cols="30"
                  rows="4"
                  class="rounded border"
                ></textarea>
              </div>
              <div class="flex justify-end py-4">
                <primary-button-rounded>Review Order</primary-button-rounded>
              </div>
            </checkout-collapse>
            <!-- end -->
          </div>
          <!-- end -->
          <!-- Order Summary -->
          <div class="flex flex-col gap-6">
            <div class="p-4 bg-white w-96 flex flex-col gap-6">
              <div class="text-xl">Order Summary</div>
              <div class="divide-y">
                <div class="flex flex-col space-y-2">
                  <div class="flex items-center justify-between">
                    <div>Product total (3)</div>
                    <div>14,000.00</div>
                  </div>
                  <div class="flex items-center justify-between">
                    <div>Shipping & Taxes</div>
                    <div>750.00</div>
                  </div>
                  <div class="flex items-center justify-between">
                    <div>Discount</div>
                    <div>0.00</div>
                  </div>
                </div>
                <div>
                  <div class="flex items-center justify-between py-2">
                    <div>Sub-Total</div>
                    <div class="font-bold">15,050.00</div>
                  </div>
                </div>
                <div>
                  <div class="flex items-center justify-between py-2">
                    <div>Total</div>
                    <div class="font-bold">15,050.00</div>
                  </div>
                </div>
              </div>

              <div class="flex items-center justify-end py-6">
                <nuxt-link to="confirm_order">
                  <primary-button-rounded>Checkout</primary-button-rounded>
                </nuxt-link>
              </div>
            </div>

            <!-- cards -->
            <div>
              <svg
                width="283"
                height="30"
                viewBox="0 0 283 30"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
              >
                <rect width="283" height="30" fill="url(#pattern0)" />
                <defs>
                  <pattern
                    id="pattern0"
                    patternContentUnits="objectBoundingBox"
                    width="1"
                    height="1"
                  >
                    <use
                      xlink:href="#image0"
                      transform="scale(0.00331126 0.03125)"
                    />
                  </pattern>
                  <image
                    id="image0"
                    width="302"
                    height="32"
                    xlink:href="data:image/png;base64,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"
                  />
                </defs>
              </svg>
            </div>
            <!-- end -->

            <div class="font-bold">Need any assistance ?</div>
            <div class="underline text-blue-600">
              Send green eagle support a mail
            </div>
            <div class="underline text-blue-600">
              Message admin on social media
            </div>
          </div>
        </section>
        <!-- end  -->
      </div>
    </main>
  </div>
</template>

<script>
import CheckoutCollapse from "../components/CheckoutCollapse.vue";
import PrimaryButtonRounded from "../components/PrimaryButtonRounded.vue";
import TextInput from "../components/TextInput.vue";
export default {
  components: { CheckoutCollapse, TextInput, PrimaryButtonRounded },
};
</script>

<style lang="scss" sc,
    PrimaryButtonRoundedoped>
</style>