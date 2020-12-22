<template>
  <div>
    <main>
      <div>
        <!-- add review -->
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
              class="absolute inset-0 bg-black opacity-25"
              tabindex="0"
            ></div>
          </div>
        </transition>
        <div
          class="transform top-0 right-0 fixed h-screen overflow-scroll ease-in-out transition-all duration-300 z-30"
          :class="!isOpen ? ' translate-x-96' : '-translate-x-0'"
        >
          <add-review></add-review>
        </div>
        <!-- end -->
        <!-- requestQuote -->
        <transition
          enter-class="opacity-0"
          enter-active-class="ease-out transition-medium"
          enter-to-class="opacity-100"
          leave-class="opacity-100"
          leave-active-class="ease-out transition-medium"
          leave-to-class="opacity-0"
        >
          <div
            @keydown.esc="isRequestQuote = false"
            v-show="isRequestQuote"
            class="z-10 fixed inset-0 transition-opacity"
          >
            <div
              @click="isRequestQuote = false"
              class="absolute inset-0 bg-black opacity-25"
              tabindex="0"
            ></div>
          </div>
        </transition>
        <div
          class="transform top-0 right-0 fixed h-screen overflow-scroll ease-in-out transition-all duration-300 z-30"
          :class="!isRequestQuote ? ' translate-x-96' : '-translate-x-0'"
        >
          <request-quote></request-quote>
        </div>
        <!-- end  -->
        <!-- image page -->
        <div class="py-10 px-20 flex flex-col">
          <div class="flex justify-between">
            <nuxt-link to="store" class="flex items-center gap-2">
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
              Back to store
            </nuxt-link>
            <div>
              <svg
                width="64"
                height="24"
                viewBox="0 0 64 24"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <rect
                  opacity="0.1"
                  width="24"
                  height="24"
                  rx="3"
                  fill="#455065"
                />
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M12 6.8175C12.8175 5.8575 14.07 5.25 15.375 5.25C17.685 5.25 19.5 7.065 19.5 9.375C19.5 12.2077 16.9542 14.5162 13.097 18.0139L13.0875 18.0225L12 19.0125L10.9125 18.03L10.8829 18.0031C7.03697 14.5082 4.5 12.2027 4.5 9.375C4.5 7.065 6.315 5.25 8.625 5.25C9.93 5.25 11.1825 5.8575 12 6.8175ZM12 16.9875L12.075 16.9125C15.645 13.68 18 11.5425 18 9.375C18 7.875 16.875 6.75 15.375 6.75C14.22 6.75 13.095 7.4925 12.705 8.52H11.3025C10.905 7.4925 9.78 6.75 8.625 6.75C7.125 6.75 6 7.875 6 9.375C6 11.5425 8.355 13.68 11.925 16.9125L12 16.9875Z"
                  fill="#455065"
                />
                <rect
                  opacity="0.1"
                  x="40"
                  width="24"
                  height="24"
                  rx="3"
                  fill="#455065"
                />
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M52 9.75V7.5C49.5175 7.5 47.5 9.5175 47.5 12C47.5 12.7575 47.6875 13.4775 48.025 14.1L46.93 15.195C46.345 14.2725 46 13.1775 46 12C46 8.685 48.685 6 52 6V3.75L55 6.75L52 9.75ZM55.975 9.9L57.07 8.805C57.655 9.7275 58 10.8225 58 12C58 15.315 55.315 18 52 18V20.25L49 17.25L52 14.25V16.5C54.4825 16.5 56.5 14.4825 56.5 12C56.5 11.2425 56.305 10.53 55.975 9.9Z"
                  fill="#455065"
                />
              </svg>
            </div>
          </div>
          <div
            class="w-full flex items-start justify-center min-h-96 py-10 px-20"
          >
            <div class="w-3/5 flex-none flex gap-10">
              <div class="flex flex-col gap-6">
                <div class="border w-24 h-32 border-primary">
                  <img src="/product.jpg" alt="" class="h-full w-full" />
                </div>
                <div class="border w-24 h-32 border-gray-100">
                  <img src="/product.jpg" alt="" class="h-full w-full" />
                </div>
                <div class="border w-24 h-32 border-gray-50">
                  <img src="/product.jpg" alt="" class="h-full w-full" />
                </div>
              </div>
              <div
                class="w-96 h-full flex items-center justify-center top-0 left-0 right-0 bottom-0"
              >
                <div>
                  <img
                    src="https://www.distrelec.biz/Web/WebShopImages/landscape_large/4-/01/Siemens-5SL4306-6-30137424-01.jpg"
                  />
                </div>
              </div>
            </div>

            <!-- text -->
            <div class="flex flex-col justify-start gap-4">
              <div class="flex items-center gap-2 text-sm">
                <svg
                  width="14"
                  height="14"
                  viewBox="0 0 14 14"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle opacity="0.2" cx="7" cy="7" r="7" fill="#1FBE5D" />
                  <circle cx="7" cy="7" r="4" fill="#1FBE5D" />
                </svg>
                12 quantity In Stock
              </div>
              <div class="text-xl">
                General Electric V07106 Circuit Breaker ...
              </div>
              <div class="py-2 flex items-center gap-4">
                <svg
                  width="107"
                  height="15"
                  viewBox="0 0 107 15"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M76.5 10.7937L80.3625 13.125L79.3375 8.73125L82.75 5.775L78.2563 5.39375L76.5 1.25L74.7438 5.39375L70.25 5.775L73.6625 8.73125L72.6375 13.125L76.5 10.7937Z"
                    fill="#F3B743"
                  />
                  <path
                    d="M53.5 10.7937L57.3625 13.125L56.3375 8.73125L59.75 5.775L55.2563 5.39375L53.5 1.25L51.7438 5.39375L47.25 5.775L50.6625 8.73125L49.6375 13.125L53.5 10.7937Z"
                    fill="#F3B743"
                  />
                  <path
                    d="M30.5 10.7937L34.3625 13.125L33.3375 8.73125L36.75 5.775L32.2563 5.39375L30.5 1.25L28.7438 5.39375L24.25 5.775L27.6625 8.73125L26.6375 13.125L30.5 10.7937Z"
                    fill="#F3B743"
                  />
                  <path
                    d="M7.5 10.7937L11.3625 13.125L10.3375 8.73125L13.75 5.775L9.25625 5.39375L7.5 1.25L5.74375 5.39375L1.25 5.775L4.6625 8.73125L3.6375 13.125L7.5 10.7937Z"
                    fill="#F3B743"
                  />
                  <path
                    d="M99.5 10.7937L103.363 13.125L102.337 8.73125L105.75 5.775L101.256 5.39375L99.5 1.25L97.7438 5.39375L93.25 5.775L96.6625 8.73125L95.6375 13.125L99.5 10.7937Z"
                    fill="#F2F2F2"
                  />
                </svg>
                4 Reviews
                <div @click="drawer" class="underline text-primary">
                  Write a review
                </div>
              </div>
              <div class="text-gray-500">Description</div>
              <div>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam
                molestie, nulla id scelerisque luctus, odio nisi consequat erat,
                eu vestibulum velit massa vel felis.
              </div>
              <div>
                <p class="text-gray-500">Brand:</p>
                General electric
              </div>
              <div>
                <p class="text-gray-500">Product code:</p>
                V07106
              </div>
              <div class="flex items-center gap-10">
                <increase></increase>
                <div
                  @click="requestQuote"
                  class="rounded bg-primary py-4 px-6 flex-none text-white"
                >
                  Request quote
                </div>
                <nuxt-link to="compair_product" class="border-2 rounded p-4"
                  >Compare</nuxt-link
                >
              </div>
            </div>
          </div>
        </div>
        <!-- end image page -->
        <!-- tab -->
        <product-details-nav
          :tabs="['Description', 'Review (4)']"
          :selected="selected"
          @selected="setSelected"
        >
          <product-detials-tab
            :isSelected="selected === 'Description'"
          ></product-detials-tab>
          <product-detials-tab :isSelected="selected === 'Review (4)'">
            <!-- review -->
            <div class="flex">
              <div class="w-1/2 flex flex-col none px-14 py-10">
                <div class="flex gap-10">
                  <div class="flex flex-col">
                    <div class="text-4xl">4.5 / 5</div>
                    <div>
                      <svg
                        width="114"
                        height="18"
                        viewBox="0 0 114 18"
                        fill="none"
                        xmlns="http://www.w3.org/2000/svg"
                      >
                        <path
                          d="M81 12.9525L85.635 15.75L84.405 10.4775L88.5 6.93L83.1075 6.4725L81 1.5L78.8925 6.4725L73.5 6.93L77.595 10.4775L76.365 15.75L81 12.9525Z"
                          fill="#F3B743"
                        />
                        <path
                          d="M57 12.9525L61.635 15.75L60.405 10.4775L64.5 6.93L59.1075 6.4725L57 1.5L54.8925 6.4725L49.5 6.93L53.595 10.4775L52.365 15.75L57 12.9525Z"
                          fill="#F3B743"
                        />
                        <path
                          d="M33 12.9525L37.635 15.75L36.405 10.4775L40.5 6.93L35.1075 6.4725L33 1.5L30.8925 6.4725L25.5 6.93L29.595 10.4775L28.365 15.75L33 12.9525Z"
                          fill="#F3B743"
                        />
                        <path
                          d="M9 12.9525L13.635 15.75L12.405 10.4775L16.5 6.93L11.1075 6.4725L9 1.5L6.8925 6.4725L1.5 6.93L5.595 10.4775L4.365 15.75L9 12.9525Z"
                          fill="#F3B743"
                        />
                        <path
                          d="M105 12.9525L109.635 15.75L108.405 10.4775L112.5 6.93L107.108 6.4725L105 1.5L102.892 6.4725L97.5 6.93L101.595 10.4775L100.365 15.75L105 12.9525Z"
                          fill="#F2F2F2"
                        />
                      </svg>
                    </div>
                    <div>4 Ratings</div>
                  </div>
                  <div>
                    <svg
                      width="260"
                      height="197"
                      viewBox="0 0 260 197"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M30 189.953L34.635 192.75L33.405 187.477L37.5 183.93L32.1075 183.472L30 178.5L27.8925 183.472L22.5 183.93L26.595 187.477L25.365 192.75L30 189.953Z"
                        fill="#F3B743"
                      />
                      <path
                        d="M50.576 180.321C48.6153 182.304 47.635 184.458 47.635 186.781C47.635 189.104 48.6153 191.258 50.576 193.241L49.607 193.921C48.4963 192.912 47.6577 191.796 47.091 190.572C46.5243 189.348 46.241 188.084 46.241 186.781C46.241 185.466 46.5243 184.203 47.091 182.99C47.6577 181.766 48.4963 180.644 49.607 179.624L50.576 180.321ZM55.6722 181.12C56.9642 181.12 57.9842 181.596 58.7322 182.548C59.4802 183.5 59.8542 184.871 59.8542 186.662C59.8542 188.441 59.4802 189.807 58.7322 190.759C57.9842 191.711 56.9642 192.187 55.6722 192.187C54.3802 192.187 53.3546 191.717 52.5952 190.776C51.8472 189.835 51.4732 188.464 51.4732 186.662C51.4732 184.849 51.8472 183.472 52.5952 182.531C53.3546 181.59 54.3802 181.12 55.6722 181.12ZM58.4602 186.662C58.4602 185.268 58.2222 184.203 57.7462 183.466C57.2702 182.718 56.5732 182.344 55.6552 182.344C54.7486 182.344 54.0572 182.718 53.5812 183.466C53.1052 184.203 52.8672 185.268 52.8672 186.662C52.8672 188.045 53.1052 189.11 53.5812 189.858C54.0572 190.595 54.7486 190.963 55.6552 190.963C56.5732 190.963 57.2702 190.595 57.7462 189.858C58.2222 189.11 58.4602 188.045 58.4602 186.662ZM60.7227 193.241C62.6833 191.258 63.6637 189.104 63.6637 186.781C63.6637 184.458 62.6833 182.304 60.7227 180.321L61.6917 179.624C62.8023 180.644 63.641 181.766 64.2077 182.99C64.7743 184.203 65.0577 185.466 65.0577 186.781C65.0577 188.084 64.7743 189.348 64.2077 190.572C63.641 191.796 62.8023 192.912 61.6917 193.921L60.7227 193.241Z"
                        fill="#455065"
                      />
                      <rect
                        x="90"
                        y="184"
                        width="170"
                        height="5"
                        rx="2.5"
                        fill="#F6F6F6"
                      />
                      <path
                        d="M30 145.953L34.635 148.75L33.405 143.477L37.5 139.93L32.1075 139.472L30 134.5L27.8925 139.472L22.5 139.93L26.595 143.477L25.365 148.75L30 145.953Z"
                        fill="#F3B743"
                      />
                      <path
                        d="M50.576 136.321C48.6153 138.304 47.635 140.458 47.635 142.781C47.635 145.104 48.6153 147.258 50.576 149.241L49.607 149.921C48.4963 148.912 47.6577 147.796 47.091 146.572C46.5243 145.348 46.241 144.084 46.241 142.781C46.241 141.466 46.5243 140.203 47.091 138.99C47.6577 137.766 48.4963 136.644 49.607 135.624L50.576 136.321ZM55.6722 137.12C56.9642 137.12 57.9842 137.596 58.7322 138.548C59.4802 139.5 59.8542 140.871 59.8542 142.662C59.8542 144.441 59.4802 145.807 58.7322 146.759C57.9842 147.711 56.9642 148.187 55.6722 148.187C54.3802 148.187 53.3546 147.717 52.5952 146.776C51.8472 145.835 51.4732 144.464 51.4732 142.662C51.4732 140.849 51.8472 139.472 52.5952 138.531C53.3546 137.59 54.3802 137.12 55.6722 137.12ZM58.4602 142.662C58.4602 141.268 58.2222 140.203 57.7462 139.466C57.2702 138.718 56.5732 138.344 55.6552 138.344C54.7486 138.344 54.0572 138.718 53.5812 139.466C53.1052 140.203 52.8672 141.268 52.8672 142.662C52.8672 144.045 53.1052 145.11 53.5812 145.858C54.0572 146.595 54.7486 146.963 55.6552 146.963C56.5732 146.963 57.2702 146.595 57.7462 145.858C58.2222 145.11 58.4602 144.045 58.4602 142.662ZM60.7227 149.241C62.6833 147.258 63.6637 145.104 63.6637 142.781C63.6637 140.458 62.6833 138.304 60.7227 136.321L61.6917 135.624C62.8023 136.644 63.641 137.766 64.2077 138.99C64.7743 140.203 65.0577 141.466 65.0577 142.781C65.0577 144.084 64.7743 145.348 64.2077 146.572C63.641 147.796 62.8023 148.912 61.6917 149.921L60.7227 149.241Z"
                        fill="#455065"
                      />
                      <rect
                        x="90"
                        y="140"
                        width="170"
                        height="5"
                        rx="2.5"
                        fill="#F6F6F6"
                      />
                      <path
                        d="M30 101.953L34.635 104.75L33.405 99.4775L37.5 95.93L32.1075 95.4725L30 90.5L27.8925 95.4725L22.5 95.93L26.595 99.4775L25.365 104.75L30 101.953Z"
                        fill="#F3B743"
                      />
                      <path
                        d="M50.576 92.321C48.6153 94.3043 47.635 96.4577 47.635 98.781C47.635 101.104 48.6153 103.258 50.576 105.241L49.607 105.921C48.4963 104.912 47.6577 103.796 47.091 102.572C46.5243 101.348 46.241 100.084 46.241 98.781C46.241 97.4663 46.5243 96.2027 47.091 94.99C47.6577 93.766 48.4963 92.644 49.607 91.624L50.576 92.321ZM55.6722 93.12C56.9642 93.12 57.9842 93.596 58.7322 94.548C59.4802 95.5 59.8542 96.8713 59.8542 98.662C59.8542 100.441 59.4802 101.807 58.7322 102.759C57.9842 103.711 56.9642 104.187 55.6722 104.187C54.3802 104.187 53.3546 103.717 52.5952 102.776C51.8472 101.835 51.4732 100.464 51.4732 98.662C51.4732 96.8487 51.8472 95.4717 52.5952 94.531C53.3546 93.5903 54.3802 93.12 55.6722 93.12ZM58.4602 98.662C58.4602 97.268 58.2222 96.2027 57.7462 95.466C57.2702 94.718 56.5732 94.344 55.6552 94.344C54.7486 94.344 54.0572 94.718 53.5812 95.466C53.1052 96.2027 52.8672 97.268 52.8672 98.662C52.8672 100.045 53.1052 101.11 53.5812 101.858C54.0572 102.595 54.7486 102.963 55.6552 102.963C56.5732 102.963 57.2702 102.595 57.7462 101.858C58.2222 101.11 58.4602 100.045 58.4602 98.662ZM60.7227 105.241C62.6833 103.258 63.6637 101.104 63.6637 98.781C63.6637 96.4577 62.6833 94.3043 60.7227 92.321L61.6917 91.624C62.8023 92.644 63.641 93.766 64.2077 94.99C64.7743 96.2027 65.0577 97.4663 65.0577 98.781C65.0577 100.084 64.7743 101.348 64.2077 102.572C63.641 103.796 62.8023 104.912 61.6917 105.921L60.7227 105.241Z"
                        fill="#455065"
                      />
                      <rect
                        x="90"
                        y="96"
                        width="170"
                        height="5"
                        rx="2.5"
                        fill="#F6F6F6"
                      />
                      <path
                        d="M30 57.9525L34.635 60.75L33.405 55.4775L37.5 51.93L32.1075 51.4725L30 46.5L27.8925 51.4725L22.5 51.93L26.595 55.4775L25.365 60.75L30 57.9525Z"
                        fill="#F3B743"
                      />
                      <path
                        d="M50.576 48.321C48.6153 50.3043 47.635 52.4577 47.635 54.781C47.635 57.1043 48.6153 59.2577 50.576 61.241L49.607 61.921C48.4963 60.9123 47.6577 59.796 47.091 58.572C46.5243 57.348 46.241 56.0843 46.241 54.781C46.241 53.4663 46.5243 52.2027 47.091 50.99C47.6577 49.766 48.4963 48.644 49.607 47.624L50.576 48.321ZM51.4392 50.14C52.1986 50.038 52.8616 49.749 53.4282 49.273H54.5162V60H53.1902V50.871C52.6236 51.2337 52.0399 51.432 51.4392 51.466V50.14ZM56.2568 61.241C58.2175 59.2577 59.1978 57.1043 59.1978 54.781C59.1978 52.4577 58.2175 50.3043 56.2568 48.321L57.2258 47.624C58.3365 48.644 59.1752 49.766 59.7418 50.99C60.3085 52.2027 60.5918 53.4663 60.5918 54.781C60.5918 56.0843 60.3085 57.348 59.7418 58.572C59.1752 59.796 58.3365 60.9123 57.2258 61.921L56.2568 61.241Z"
                        fill="#455065"
                      />
                      <rect
                        x="90"
                        y="52"
                        width="170"
                        height="5"
                        rx="2.5"
                        fill="#F6F6F6"
                      />
                      <rect
                        x="90"
                        y="52"
                        width="20"
                        height="5"
                        rx="2.5"
                        fill="#F3B743"
                      />
                      <path
                        d="M30 13.9525L34.635 16.75L33.405 11.4775L37.5 7.93L32.1075 7.4725L30 2.5L27.8925 7.4725L22.5 7.93L26.595 11.4775L25.365 16.75L30 13.9525Z"
                        fill="#F3B743"
                      />
                      <path
                        d="M12.259 12.532C12.259 11.1833 11.3807 10.509 9.624 10.509H6.751L7.21 5.307H13.143V6.531H8.502L8.213 9.608C8.80233 9.506 9.36333 9.455 9.896 9.455C11.0633 9.455 11.9813 9.71567 12.65 10.237C13.3187 10.747 13.653 11.5233 13.653 12.566C13.653 13.6087 13.3017 14.4757 12.599 15.167C11.8963 15.847 10.9897 16.187 9.879 16.187C8.76833 16.187 7.86167 15.9093 7.159 15.354C6.45633 14.7873 6.105 14.011 6.105 13.025H7.448C7.448 13.9543 7.924 14.5607 8.876 14.844C9.17067 14.9233 9.49367 14.963 9.845 14.963C10.5703 14.963 11.154 14.7363 11.596 14.283C12.038 13.8183 12.259 13.2347 12.259 12.532Z"
                        fill="#455065"
                      />
                      <path
                        d="M50.576 4.321C48.6153 6.30433 47.635 8.45767 47.635 10.781C47.635 13.1043 48.6153 15.2577 50.576 17.241L49.607 17.921C48.4963 16.9123 47.6577 15.796 47.091 14.572C46.5243 13.348 46.241 12.0843 46.241 10.781C46.241 9.46633 46.5243 8.20267 47.091 6.99C47.6577 5.766 48.4963 4.644 49.607 3.624L50.576 4.321ZM59.1912 8.044C59.1912 9.17733 58.5679 9.965 57.3212 10.407C58.0012 10.5997 58.5509 10.917 58.9702 11.359C59.3896 11.801 59.5992 12.3677 59.5992 13.059C59.5992 13.9997 59.2422 14.759 58.5282 15.337C57.8142 15.9037 56.8736 16.187 55.7062 16.187C54.5389 16.187 53.5416 15.8867 52.7142 15.286C51.8982 14.674 51.4902 13.8183 51.4902 12.719H52.8842C52.9069 13.4443 53.1732 13.9997 53.6832 14.385C54.2046 14.7703 54.8619 14.963 55.6552 14.963C56.4486 14.963 57.0606 14.776 57.4912 14.402C57.9332 14.0167 58.1542 13.5463 58.1542 12.991C58.1542 12.4243 57.9446 11.9653 57.5252 11.614C57.1059 11.2513 56.4259 11.07 55.4852 11.07H54.2612V9.999H55.0942C55.9102 9.999 56.5562 9.84033 57.0322 9.523C57.5082 9.19433 57.7462 8.758 57.7462 8.214C57.7462 7.67 57.5536 7.22233 57.1682 6.871C56.7829 6.51967 56.2729 6.344 55.6382 6.344C55.0036 6.344 54.4709 6.45733 54.0402 6.684C53.6209 6.89933 53.3376 7.30733 53.1902 7.908H51.7962C51.9209 6.96733 52.3119 6.27033 52.9692 5.817C53.6266 5.35233 54.4709 5.12 55.5022 5.12C56.5449 5.12 57.4176 5.39767 58.1202 5.953C58.8342 6.497 59.1912 7.194 59.1912 8.044ZM60.6728 17.241C62.6335 15.2577 63.6138 13.1043 63.6138 10.781C63.6138 8.45767 62.6335 6.30433 60.6728 4.321L61.6418 3.624C62.7525 4.644 63.5912 5.766 64.1578 6.99C64.7245 8.20267 65.0078 9.46633 65.0078 10.781C65.0078 12.0843 64.7245 13.348 64.1578 14.572C63.5912 15.796 62.7525 16.9123 61.6418 17.921L60.6728 17.241Z"
                        fill="#455065"
                      />
                      <rect
                        x="90"
                        y="8"
                        width="170"
                        height="5"
                        rx="2.5"
                        fill="#F6F6F6"
                      />
                      <rect
                        x="90"
                        y="8"
                        width="130"
                        height="5"
                        rx="2.5"
                        fill="#F3B743"
                      />
                      <path
                        d="M0.833 187.14C1.59233 187.038 2.25533 186.749 2.822 186.273H3.91V197H2.584V187.871C2.01733 188.234 1.43367 188.432 0.833 188.466V187.14Z"
                        fill="#455065"
                      />
                      <path
                        d="M2.431 151.759H8.636V153H1.088V151.419C1.088 150.161 1.564 149.237 2.516 148.648C2.822 148.455 3.162 148.285 3.536 148.138L5.644 147.288C6.732 146.857 7.276 146.149 7.276 145.163C7.276 144.619 7.089 144.177 6.715 143.837C6.341 143.486 5.814 143.31 5.134 143.31C4.46533 143.31 3.91567 143.452 3.485 143.735C3.06567 144.018 2.822 144.443 2.754 145.01H1.275C1.33167 144.081 1.70567 143.367 2.397 142.868C3.08833 142.369 3.97233 142.12 5.049 142.12C6.137 142.12 7.021 142.415 7.701 143.004C8.381 143.593 8.721 144.324 8.721 145.197C8.721 146.058 8.49433 146.744 8.041 147.254C7.599 147.764 6.987 148.172 6.205 148.478L4.046 149.345C3.502 149.572 3.094 149.832 2.822 150.127C2.56133 150.41 2.431 150.784 2.431 151.249V151.759Z"
                        fill="#455065"
                      />
                      <path
                        d="M8.585 101.044C8.585 102.177 7.96167 102.965 6.715 103.407C7.395 103.6 7.94467 103.917 8.364 104.359C8.78333 104.801 8.993 105.368 8.993 106.059C8.993 107 8.636 107.759 7.922 108.337C7.208 108.904 6.26733 109.187 5.1 109.187C3.93267 109.187 2.93533 108.887 2.108 108.286C1.292 107.674 0.884 106.818 0.884 105.719H2.278C2.30067 106.444 2.567 107 3.077 107.385C3.59833 107.77 4.25567 107.963 5.049 107.963C5.84233 107.963 6.45433 107.776 6.885 107.402C7.327 107.017 7.548 106.546 7.548 105.991C7.548 105.424 7.33833 104.965 6.919 104.614C6.49967 104.251 5.81967 104.07 4.879 104.07H3.655V102.999H4.488C5.304 102.999 5.95 102.84 6.426 102.523C6.902 102.194 7.14 101.758 7.14 101.214C7.14 100.67 6.94733 100.222 6.562 99.871C6.17667 99.5197 5.66667 99.344 5.032 99.344C4.39733 99.344 3.86467 99.4573 3.434 99.684C3.01467 99.8993 2.73133 100.307 2.584 100.908H1.19C1.31467 99.9673 1.70567 99.2703 2.363 98.817C3.02033 98.3523 3.86467 98.12 4.896 98.12C5.93867 98.12 6.81133 98.3977 7.514 98.953C8.228 99.497 8.585 100.194 8.585 101.044Z"
                        fill="#455065"
                      />
                      <path
                        d="M7.276 54.154V61.26H9.129V62.416H7.276V65H5.967V62.416H0.442V61.379L6.035 54.154H7.276ZM2.04 61.379H6.001V56.279L2.04 61.379Z"
                        fill="#455065"
                      />
                    </svg>
                  </div>
                </div>
                <div class="my-10 flex justify-center">
                  <input
                    type="button"
                    value="Write a review"
                    class="rounded border py-2 px-6 inline-block bg-white"
                    @click="drawer"
                  />
                </div>
              </div>
              <div class="w-1/2 flex flex-col none px-14 py-10 gap-10">
                <!-- single review -->
                <div class="flex gap-4">
                  <div>
                    <svg
                      width="40"
                      height="40"
                      viewBox="0 0 40 40"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <circle
                        opacity="0.597052"
                        cx="20"
                        cy="20"
                        r="20"
                        fill="#8B41E7"
                        fill-opacity="0.2"
                      />
                      <path
                        d="M17.86 22.27C17.86 23.3 17.625 24.04 17.155 24.49C16.695 24.94 16.105 25.165 15.385 25.165C14.665 25.165 13.91 24.955 13.12 24.535V23.305C13.82 23.785 14.475 24.025 15.085 24.025C15.705 24.025 16.125 23.875 16.345 23.575C16.565 23.275 16.675 22.84 16.675 22.27V15.565H17.86V22.27ZM25.2045 17.86C25.0345 16.94 24.3595 16.48 23.1795 16.48C22.5495 16.48 22.0645 16.62 21.7245 16.9C21.3845 17.17 21.2145 17.5 21.2145 17.89C21.2145 18.27 21.3195 18.56 21.5295 18.76C21.7395 18.96 22.0795 19.135 22.5495 19.285L24.5145 19.96C25.1845 20.19 25.7145 20.505 26.1045 20.905C26.5045 21.305 26.7045 21.87 26.7045 22.6C26.7045 23.32 26.3945 23.93 25.7745 24.43C25.1545 24.92 24.3245 25.165 23.2845 25.165C22.2445 25.165 21.3895 24.905 20.7195 24.385C20.0595 23.855 19.7195 23.115 19.6995 22.165H20.8545C20.8545 22.785 21.0695 23.26 21.4995 23.59C21.9395 23.92 22.4995 24.085 23.1795 24.085C23.8695 24.085 24.4145 23.935 24.8145 23.635C25.2145 23.325 25.4145 22.965 25.4145 22.555C25.4145 22.135 25.2895 21.805 25.0395 21.565C24.7995 21.325 24.4395 21.125 23.9595 20.965L22.2945 20.35C21.5145 20.09 20.9245 19.78 20.5245 19.42C20.1245 19.06 19.9245 18.535 19.9245 17.845C19.9245 17.145 20.2045 16.565 20.7645 16.105C21.3245 15.635 22.1095 15.4 23.1195 15.4C24.1295 15.4 24.8995 15.625 25.4295 16.075C25.9695 16.515 26.2795 17.11 26.3595 17.86H25.2045Z"
                        fill="#455065"
                      />
                    </svg>
                  </div>
                  <div class="flex flex-col gap-4">
                    <div class="flex items-center">John Stones</div>
                    <four-stars></four-stars>
                    <div>
                      Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                      Nullam molestie, nulla id scelerisque luctus, odio nisi
                      consequat erat, eu vestibulum velit massa vel felis.
                    </div>
                    <div class="flex items-center py-4 text-sm text-gray-300">
                      <div>09-25-2020</div>
                      <div>11 : 20PM</div>
                    </div>
                  </div>
                </div>
                <!-- end single review -->
                <!-- single review -->
                <div class="flex gap-4">
                  <div>
                    <svg
                      width="40"
                      height="40"
                      viewBox="0 0 40 40"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <circle
                        opacity="0.597052"
                        cx="20"
                        cy="20"
                        r="20"
                        fill="#2AA580"
                        fill-opacity="0.2"
                      />
                      <path
                        d="M13.5 15.565H19.305V16.585H14.685V19.75H19.035V20.755H14.685V23.965H19.305V25H13.5V15.565ZM24.8079 15.4C25.8179 15.4 26.6279 15.655 27.2379 16.165C27.8579 16.665 28.2829 17.32 28.5129 18.13L27.2379 18.385C27.0379 17.795 26.7229 17.33 26.2929 16.99C25.8729 16.64 25.3779 16.465 24.8079 16.465C24.0179 16.465 23.3629 16.795 22.8429 17.455C22.3229 18.115 22.0629 19.035 22.0629 20.215C22.0629 21.385 22.2929 22.325 22.7529 23.035C23.2229 23.745 23.9079 24.1 24.8079 24.1C25.5579 24.1 26.1479 23.905 26.5779 23.515C27.0179 23.115 27.2379 22.59 27.2379 21.94H28.5129C28.5129 22.93 28.1729 23.715 27.4929 24.295C26.8229 24.875 25.8979 25.165 24.7179 25.165C23.5479 25.165 22.5979 24.715 21.8679 23.815C21.1479 22.915 20.7879 21.71 20.7879 20.2C20.7879 18.69 21.1629 17.515 21.9129 16.675C22.6629 15.825 23.6279 15.4 24.8079 15.4Z"
                        fill="#455065"
                      />
                    </svg>
                  </div>
                  <div class="flex flex-col gap-4">
                    <div class="flex items-center">Edith Car</div>
                    <four-stars></four-stars>
                    <div>
                      Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                      Nullam molestie, nulla id scelerisque luctus, odio nisi
                      consequat erat, eu vestibulum velit massa vel felis.
                    </div>
                    <div class="flex items-center py-4 text-sm text-gray-300">
                      <div>09-25-2020</div>
                      <div>11 : 20PM</div>
                    </div>
                  </div>
                </div>
                <!-- end single review -->

                <!-- single review -->
                <div class="flex gap-4">
                  <div>
                    <svg
                      width="40"
                      height="40"
                      viewBox="0 0 40 40"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <circle
                        cx="20"
                        cy="20"
                        r="20"
                        fill="#E74141"
                        fill-opacity="0.15"
                      />
                      <path
                        d="M15.7 23.965H19.9V25H14.515V15.565H15.7V23.965ZM22.3166 23.965H26.5166V25H21.1316V15.565H22.3166V23.965Z"
                        fill="#455065"
                      />
                    </svg>
                  </div>
                  <div class="flex flex-col gap-4">
                    <div class="flex items-center">Lida Lynch</div>
                    <four-stars></four-stars>
                    <div>
                      Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                      Nullam molestie, nulla id scelerisque luctus, odio nisi
                      consequat erat, eu vestibulum velit massa vel felis.
                    </div>
                    <div class="flex items-center py-4 text-sm text-gray-300">
                      <div>09-25-2020</div>
                      <div>11 : 20PM</div>
                    </div>
                  </div>
                </div>
                <!-- end single review -->
              </div>
            </div>
            <!-- review -->
          </product-detials-tab>
        </product-details-nav>
        <!-- end tab  -->
        <div class="flex items-center flex-col text-xl">
          <p class="p-10">Other Products In The Same Category</p>
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
    </main>
  </div>
</template>

<script>
import AddReview from "../components/AddReview.vue";
import FourStars from "../components/FourStars.vue";
import Increase from "../components/Increase.vue";
import ProductDetailsNav from "../components/ProductDetailsNav.vue";
import ProductDetialsTab from "../components/ProductDetialsTab.vue";
import Products from "../components/Products.vue";
export default {
  components: { ProductDetialsTab, FourStars, Products, AddReview, Increase },
  data() {
    return { selected: "Review (4)", isOpen: false, isRequestQuote: false };
  },
  methods: {
    setSelected(tab) {
      this.selected = tab;
    },
    drawer() {
      this.isOpen = !this.isOpen;
    },
    requestQuote() {
      this.isRequestQuote = !this.isRequestQuote;
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
      handler(isRequestQuote) {
        if (process.client) {
          if (isRequestQuote)
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
      if (e.keyCode == 27 && this.isRequestQuote) {
        this.isRequestQuote = false;
      }
    });
  },
};
</script>

<style  scoped>
img {
  background-size: cover;
}
</style>