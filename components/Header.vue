<template>
  <div>
    <div class="w-screen text-gray-500">
      <div class="w-screen bg-bg_pop_up">
        <div
          class="h-12 flex space-x-40 items-center content-center justify-between px-8"
        >
          <div class="h-6 flex space-x-4 items-center">
            <div class="py-1 px-2 shadow-md rounded bg-btn_pop_up text-white">
              Offers
            </div>
            <div>10% discount for all first time users</div>
          </div>
          <div class="h-6 flex divide-x divide-gray-300 space-x">
            <div class="px-3 text-sm text-gray-500">Wishlist</div>
            <div class="px-3 text-sm text-gray-500">
              <label
                for="cars"
                class="border-none focus:border-none bg-bg_pop_up"
              ></label>

              <select
                name="cars"
                id="cars"
                class="bg-bg_pop_up focus:border-gray-600"
              >
                <option value="doller">USD $</option>
                <option value="pounds">PND &#163;</option>
                <option value="nira">NGN &#8358;</option>
                <option value="euros">EUR &#8364;</option>
              </select>
            </div>
            <div class="px-3 text-sm text-gray-500">
              <label
                for="cars"
                class="border-none focus:border-none bg-bg_pop_up"
              ></label>

              <select
                name="cars"
                id="cars"
                class="bg-bg_pop_up focus:border-gray-600"
              >
                <option value="english">ENGLISH</option>
                <option value="hausa">HAUSA</option>
                <option value="yoruba">YOROBA</option>
                <option value="egbo">EGBO</option>
              </select>
            </div>
          </div>
        </div>
      </div>
      <!-- search bar -->
      <div
        class="h-20 flex content-center items-center justify-end px-10 space-x-10"
      >
        <!-- search bar -->
        <div class="h-10 border w-7/12 flex content-center rounded">
          <!-- dropdown -->
          <div class="px-3 text-sm text-gray-500 h-full border-r-2">
            <label for="cars" class="focus:border-none bg-bg_pop_up"></label>

            <select
              name="cars"
              id="cars"
              class="focus:border-gray-600 h-full focus:outline-none flex-none"
            >
              <option value="Mechcanical">Mechcanical</option>
              <option value="Systems">Systems and solutions</option>
              <option value="Electrical">Electrical</option>
              <option value="Power">Power supplies</option>
              <option value="Other">Other</option>
              <option value="Shop by brand">Shop by brands</option>
            </select>
          </div>
          <!-- end -->
          <!-- input  -->
          <div class="flex-grow">
            <input
              type="text"
              name=""
              id=""
              class="h-full w-full p-2 border-none focus:outline-none"
              placeholder="Search for industrial products or search by part number"
            />
          </div>
          <!-- edn -->
          <!-- search icon -->
          <div class="flex-none w-10 text-sm">
            <div class="p-2 text-primary">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                fill="currentColor"
              >
                <path
                  fill-rule="evenodd"
                  d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z"
                  clip-rule="evenodd"
                />
              </svg>
            </div>
          </div>
          <!-- end -->
        </div>
        <!-- cart and sign in -->
        <div class="flex flex-none h-10 text-gray-500 w-80">
          <!-- my cart -->
          <div class="grid grid-rows-3 grid-flow-col gap-x-3 gap-y-5">
            <div class="row-span-3 w-8 ustify-self-center">
              <!-- cart icon -->
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
                />
              </svg>
            </div>
            <div class="col-span-2 font-bold">My Cart</div>
            <div class="row-span-2 text-xs">0 Items $0.00</div>
          </div>
          <!-- end -->

          <!-- my account -->
          <div class="grid grid-rows-3 grid-flow-col gap-x-3 gap-y-5">
            <div class="row-span-3 w-8 ustify-self-center">
              <!-- cart icon -->
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"
                />
              </svg>
              <!-- end -->
            </div>
            <div class="col-span-2 font-bold">My Account</div>
            <div class="row-span-2 text-xs">Register & Login</div>
          </div>
          <!-- end -->
        </div>
      </div>
      <div class="h-14 bg-primary flex items-center px-8 text-white">
        <div class="border-r-2 border-gray-500 h-full flex items-center">
          <div class="w-6 h-6">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              />
            </svg>
          </div>
          <div class="px-6">Categories</div>
        </div>
        <!--  -->
        <div class="flex px-4 space-x-6 text-sm">
          <p>Mechcanical</p>
          <p>Systems and solutions</p>
          <p>Electrical</p>
          <p>Electronics</p>
          <p>Power supplies</p>
          <p>Other</p>
          <p>Shop by brands</p>
        </div>
        <!--  -->
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style >
</style>