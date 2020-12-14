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
          <li>
            <div>1. Billing Details</div>
          </li>
          <li><div>2. Shipping Details</div></li>
          <li><div>3. Delivery Method</div></li>
          <li><div>4. Payment Method</div></li>
          <li class="border-b-4 border-primary py-4">
            <div>5. Confirm Order</div>
          </li>
        </ul>
      </div>
    </div>
    <!-- end -->

    <div class="py-6 px-20 flex flex-col gap-8">
      <!-- card -->
      <div class="py-6 px-2 flex flex-col bg-white gap-6">
        <div class="px-12 text-lg">
          <p>Please confirm your order</p>
        </div>
        <div class="mx-12 w-screen">
          <table class="table-fixed text-sm">
            <thead>
              <tr class="border-b font-bold border-gray-200 text-center">
                <th class="w-52 py-2">Product Name</th>
                <th class="w-52 py-2">Model</th>
                <th class="w-52 py-2">Quantity</th>
                <th class="w-52 py-2">Unit Price ( $ )</th>
                <th class="w-52 py-2">Total ($ )</th>
              </tr>
            </thead>
            <tbody>
              <!--  -->
              <tr class="text-center border-gray-200 border-b">
                <td class="p-2">31002060011</td>
                <td class="p-2">31002060011</td>
                <td class="p-2">1</td>
                <td class="p-2">3500.00</td>
                <td class="p-2">3500.00</td>
              </tr>
              <!--  -->
              <tr class="text-center border-gray-200 border-b">
                <td class="p-2">PQMII-T20-C-A</td>
                <td class="p-2">PQMII-T20-C-A</td>
                <td class="p-2">1</td>
                <td class="p-2">5700.00</td>
                <td class="p-2">7500.00</td>
              </tr>
              <!--  -->
              <tr class="text-center border-gray-200 border-b">
                <td class="p-2">585-4UDE-3YU3IO</td>
                <td class="p-2">585-4UDE-3YU3IO</td>
                <td class="p-2">1</td>
                <td class="p-2">2300.00</td>
                <td class="p-2">2300.00</td>
              </tr>
              <!--  -->
              <tr class="text-center border-gray-200 border-b">
                <td class="p-2"></td>
                <td class="p-2"></td>
                <td class="p-2"></td>
                <td class="p-2">Sub-Total</td>
                <td class="p-2 font-bold">15,050.00</td>
              </tr>
              <!--  -->
              <tr class="text-center border-gray-200 border-b">
                <td class="p-2"></td>
                <td class="p-2"></td>
                <td class="p-2"></td>
                <td class="p-2">UPS Worldwide Express Plus</td>
                <td class="p-2 font-bold">442.00</td>
              </tr>
              <!--  -->
              <tr class="text-center">
                <td class="p-2"></td>
                <td class="p-2"></td>
                <td class="p-2"></td>
                <td class="p-2">Total</td>
                <td class="p-2 font-bold">15,050.00</td>
              </tr>
              <!--  -->
            </tbody>
          </table>
        </div>
        <!--  -->
      </div>
      <!--  -->

      <!-- end card -->

      <!-- second card -->
      <div class="py-6 px-12 grid grid-cols-2 bg-white gap-20">
        <!-- infor item -->
        <div class="font-thin flex flex-col gap-4">
          <div class="flex items-center justify-between border-b py-4">
            <p class="font-normal">Your information</p>
            <input type="button" value="Edit" class="bg-white text-primary" />
          </div>
          <div class="space-y-2">
            <p class="font-normal">Jude Ejike</p>
            <p>newjutla@ha.com</p>
            <p>(357) 734-5280</p>
          </div>
        </div>
        <!--end  -->

        <!-- infor item -->
        <div class="font-thin flex flex-col gap-4">
          <div class="flex items-center justify-between border-b py-4">
            <p class="font-normal">Card information</p>
            <input type="button" value="Edit" class="bg-white text-primary" />
          </div>
          <div class="space-y-2">
            <p>Visa card ending with 5600</p>
          </div>
        </div>
        <!--end  -->
        <!-- infor item -->
        <div class="font-thin flex flex-col gap-4">
          <div class="flex items-center justify-between border-b py-4">
            <p class="font-normal">Shipping address</p>
            <input type="button" value="Edit" class="bg-white text-primary" />
          </div>
          <div class="space-y-2">
            <p class="font-normal">Jude Ejike</p>
            <p>5 Adediran Ajao cresent</p>
            <p>Anthony Village</p>
            <p>Lagos, Nigeria.</p>
          </div>
        </div>
        <!--end  -->
      </div>
      <!-- end second card -->
      <div class="flex items-center gap-4 justify-end">
        <p>
          Can you confrirm that you have gone through your order and wish to
          proceed ?
        </p>
        <primary-button-rounded>Make payment</primary-button-rounded>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
</style>