<template>
  <div class="">
    <div class="min-h-screen border-r py-6 pl-10 pr-4 flex flex-col gap-6">
      <!-- home navigations -->
      <div class="flex divide-x divide-gray-300 space-x">
        <nuxt-link to="/" class="px-3">Home</nuxt-link>
        <nuxt-link to="store" class="px-3">Store</nuxt-link>
      </div>
      <!-- end home -->
      <!-- Shopping categories -->
      <div class="flex flex-col justify-start pl-3">
        <div class="text-lg">Shopping categories</div>
        <!-- list -->
        <div class="space-y-2 py-4">
          <!-- list item -->
          <div class="border-b flex justify-between py-2">
            <div class="font-thin">Mechcanical</div>
            <div>23</div>
          </div>
          <!-- end list item  -->
          <!-- list item -->
          <div class="border-b flex justify-between py-2">
            <div class="font-thin">Systems and solutions</div>
            <div>05</div>
          </div>
          <!-- end list item  -->
          <!-- list item -->
          <div class="border-b flex justify-between py-2">
            <div class="font-thin">Electrical</div>
            <div>02</div>
          </div>
          <!-- end list item  -->
          <!-- list item -->
          <div class="border-b flex justify-between py-2">
            <div class="font-thin">Electronics</div>
            <div>23</div>
          </div>
          <!-- end list item  -->
          <!-- list item -->
          <div class="border-b flex justify-between py-2">
            <div class="font-thin">Power supplies</div>
            <div>29</div>
          </div>
          <!-- end list item  -->
          <!-- list item -->
          <div class="border-b flex justify-between py-2">
            <div class="font-thin">Other</div>
            <div>29</div>
          </div>
          <!-- end list item  -->
          <!-- list item -->
          <div class="border-b flex justify-between py-2">
            <div class="font-thin">Shop by brands</div>
            <div>29</div>
          </div>
          <!-- end list item  -->
          <!-- list item -->
          <div class="border-b flex justify-between py-2">
            <div class="font-thin">Expert guide</div>
          </div>
          <!-- end list item  -->
        </div>
        <!-- end list -->
        <div class="font-thin py-4">Return and refund policy</div>
      </div>
      <!-- end Shopping categories -->
      <!-- range -->
      <div>
        <div class="flex justify-between">
          <div>Price range</div>
          <div class="text-red-400">APPLY</div>
        </div>
        <div class="py-3">
          <svg
            width="257"
            height="20"
            viewBox="0 0 257 20"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <rect y="7" width="257" height="6" rx="3" fill="#F2F2F2" />
            <rect y="7" width="197" height="6" rx="3" fill="#2AA580" />
            <circle cx="194" cy="10" r="10" fill="#2AA580" />
            <circle cx="64" cy="10" r="10" fill="#2AA580" />
          </svg>
        </div>

        <div class="flex justify-between">
          <input
            type="text"
            name=""
            id=""
            value="0"
            class="border rounded w-28 p-2"
          />
          <div>to</div>
          <input
            type="text"
            name=""
            id=""
            value="200"
            class="border rounded w-28 p-2"
          />
        </div>
      </div>
      <!-- end range -->

      <!-- rating -->
      <rating></rating>
      <!-- end of rating -->
    </div>
  </div>
</template>


<style lang="scss" scoped></style>;
