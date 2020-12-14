<template>
  <div class="bg-white z-10">
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
        <nuxt-link to="/">
          <img src="/logo.png" alt="" />
        </nuxt-link>
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
          <div
            @click="showCart"
            class="grid grid-rows-3 grid-flow-col gap-x-3 gap-y-5"
          >
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
            <NuxtLink to="register" class="row-span-2 text-xs"
              >Register & Login</NuxtLink
            >
          </div>
          <!-- end -->
        </div>
      </div>
      <div class="h-14 bg-primary flex items-center px-8 text-white">
        <div class="border-r-2 border-gray-500 h-full flex items-center">
          <div class="w-6 h-6" @click="drawer">
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
          <nuxt-link to="store">Mechcanical</nuxt-link>
          <nuxt-link to="store">Systems and solutions</nuxt-link>
          <nuxt-link to="store">Electrical</nuxt-link>
          <nuxt-link to="store">Electronics</nuxt-link>
          <nuxt-link to="store">Power supplies</nuxt-link>
          <nuxt-link to="store">Other</nuxt-link>
          <nuxt-link to="store">Shop by brands</nuxt-link>
        </div>
        <!--  -->
      </div>
    </div>
    <transition
      enter-class="opacity-0"
      enter-active-class="ease-out transition-medium"
      enter-to-class="opacity-100"
      leave-class="opacity-100"
      leave-active-class="ease-out transition-medium"
      leave-to-class="opacity-0"
    >
      <div
        @keydown.esc="isOpen = false"
        v-show="isOpen"
        class="z-10 fixed inset-0 transition-opacity"
      >
        <div
          @click="isOpen = false"
          class="absolute inset-0"
          tabindex="0"
        ></div>
      </div>
    </transition>
    <aside
      class="transform top-0 left-0 bg-white fixed h-screen overflow-scroll ease-in-out transition-all duration-300 z-30"
      :class="isOpen ? 'translate-x-0' : '-translate-x-full'"
    >
      <side-nav></side-nav>
    </aside>

    <transition
      enter-class="opacity-0"
      enter-active-class="ease-out transition-medium"
      enter-to-class="opacity-100"
      leave-class="opacity-100"
      leave-active-class="ease-out transition-medium"
      leave-to-class="opacity-0"
    >
      <div
        @keydown.esc="isCartSelected = false"
        v-show="isCartSelected"
        class="z-10 fixed inset-0 transition-opacity"
      >
        <div
          @click="isCartSelected = false"
          class="absolute inset-0"
          tabindex="0"
        ></div>
      </div>
    </transition>
    <div
      class="transform top-0 right-12 bg-white fixed overflow-scroll ease-in-out transition-all duration-300 z-30"
      :class="isCartSelected ? 'translate-y-28' : '-translate-y-full'"
    >
      <div class="w-96 flex flex-col p-10">
        <div class="flex items-center justify-between">
          <div>My Cart</div>
          <div>
            <svg
              width="21"
              height="20"
              viewBox="0 0 21 20"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <rect
                x="4.69678"
                y="14.1248"
                width="13.3333"
                height="1.66667"
                rx="0.833333"
                transform="rotate(-45 4.69678 14.1248)"
                fill="#2AA580"
              />
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M5.28574 5.28595C5.61118 4.96052 6.13882 4.96052 6.46426 5.28595L14.7138 13.5355C15.0393 13.861 15.0393 14.3886 14.7138 14.714C14.3884 15.0395 13.8608 15.0395 13.5353 14.714L5.28574 6.46447C4.96031 6.13903 4.96031 5.61139 5.28574 5.28595Z"
                fill="#2AA580"
              />
            </svg>
          </div>
        </div>
        <!-- cart item -->
        <div class="border-b">
          <div class="grid grid-rows-3 grid-flow-col gap-2 p-2">
            <div class="row-span-3">
              <img
                src="~/assets/images/product1.png"
                alt=""
                class="h-full w-full"
              />
            </div>
            <div class="row-span-1 text-lg">$390.00</div>
            <div class="row-span-2">
              <div class="font-thin">General Electric V07106 …</div>
              <div class="font-thin flex items-center justify-between">
                <div>Quantity: 1</div>
                <div>
                  <svg
                    width="11"
                    height="14"
                    viewBox="0 0 11 14"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      fill-rule="evenodd"
                      clip-rule="evenodd"
                      d="M8.25 0.777778L7.46429 0H3.53571L2.75 0.777778H0V2.33333H11V0.777778H8.25ZM0.785714 12.4444C0.785714 13.3 1.49286 14 2.35714 14H8.64286C9.50714 14 10.2143 13.3 10.2143 12.4444V3.11111H0.785714V12.4444ZM8.64286 4.66667H2.35714V12.4444H8.64286V4.66667Z"
                      fill="#FE5F55"
                    />
                  </svg>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!-- end -->
        <!-- cart item -->
        <div class="border-b">
          <div class="grid grid-rows-3 grid-flow-col gap-2 p-2">
            <div class="row-span-3">
              <img
                src="~/assets/images/product2.png"
                alt=""
                class="h-full w-full"
              />
            </div>
            <div class="row-span-1 text-lg">$390.00</div>
            <div class="row-span-2">
              <div class="font-thin">General Electric V07106 …</div>
              <div class="font-thin flex items-center justify-between">
                <div>Quantity: 1</div>
                <div>
                  <svg
                    width="11"
                    height="14"
                    viewBox="0 0 11 14"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      fill-rule="evenodd"
                      clip-rule="evenodd"
                      d="M8.25 0.777778L7.46429 0H3.53571L2.75 0.777778H0V2.33333H11V0.777778H8.25ZM0.785714 12.4444C0.785714 13.3 1.49286 14 2.35714 14H8.64286C9.50714 14 10.2143 13.3 10.2143 12.4444V3.11111H0.785714V12.4444ZM8.64286 4.66667H2.35714V12.4444H8.64286V4.66667Z"
                      fill="#FE5F55"
                    />
                  </svg>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!-- end -->

        <!-- subtotal -->
        <div class="flex items-center justify-between py-4">
          <div class="font-thin">Sub-total</div>
          <div class="font-bold">$980.05</div>
        </div>
        <!-- end -->
        <!-- view cart check out -->
        <div class="flex items-center justify-evenly py-4">
          <nuxt-link
            to="cart_menu"
            class="bg-primary rounded text-white py-2 px-6"
            >View Cart</nuxt-link
          >
          <div class="border rounded py-2 px-6">Checkout</div>
        </div>
        <!-- end -->
      </div>
    </div>
  </div>
</template>


<script>
import SideNav from "./SideNav.vue";
export default {
  components: { SideNav },
  data() {
    return {
      isOpen: false,
      isCartSelected: false,
    };
  },
  methods: {
    drawer() {
      this.isOpen = !this.isOpen;
    },
    showCart() {
      this.isCartSelected = !this.isCartSelected;
    },
  },
  watch: {
    isOpen: {
      immediate: true,
      handler(isOpen) {
        if (process.client) {
          if (isOpen) document.body.style.setProperty("overflow", "hidden");
          else document.body.style.removeProperty("overflow");
        }
      },
    },
    isCartSelected: {
      immediate: true,
      handler(isCartSelected) {
        if (process.client) {
          if (isCartSelected)
            document.body.style.setProperty("overflow", "hidden");
          else document.body.style.removeProperty("overflow");
        }
      },
    },
  },
  mounted() {
    document.addEventListener("keydown", (e) => {
      if (e.keyCode == 27 && this.isOpen) {
        this.isOpen = false;
      }
      if (e.keyCode == 27 && this.isCartSelected) {
        this.isCartSelected = false;
      }
    });
  },
};
</script>

<style >
</style>