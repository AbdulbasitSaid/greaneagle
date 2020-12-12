<template>
  <div>
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
      <div>
        <div class="text-lg">Product rating</div>
        <!-- stars -->
        <div>
          <!-- star -->
          <div class="flex items-center gap-4">
            <input type="checkbox" name="5" id="5" />
            <label for="5">
              <svg
                width="124"
                height="20"
                viewBox="0 0 124 20"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M88.5 14.8589L93.753 18L92.359 12.08L97 8.09684L90.8885 7.58316L88.5 2L86.1115 7.58316L80 8.09684L84.641 12.08L83.247 18L88.5 14.8589Z"
                  fill="#F3B743"
                />
                <path
                  d="M62.5 14.8589L67.753 18L66.359 12.08L71 8.09684L64.8885 7.58316L62.5 2L60.1115 7.58316L54 8.09684L58.641 12.08L57.247 18L62.5 14.8589Z"
                  fill="#F3B743"
                />
                <path
                  d="M36.5 14.8589L41.753 18L40.359 12.08L45 8.09684L38.8885 7.58316L36.5 2L34.1115 7.58316L28 8.09684L32.641 12.08L31.247 18L36.5 14.8589Z"
                  fill="#F3B743"
                />
                <path
                  d="M10.5 14.8589L15.753 18L14.359 12.08L19 8.09684L12.8885 7.58316L10.5 2L8.1115 7.58316L2 8.09684L6.641 12.08L5.247 18L10.5 14.8589Z"
                  fill="#F3B743"
                />
                <path
                  d="M114.5 14.8589L119.753 18L118.359 12.08L123 8.09684L116.889 7.58316L114.5 2L112.111 7.58316L106 8.09684L110.641 12.08L109.247 18L114.5 14.8589Z"
                  fill="#F2F2F2"
                />
                <path
                  d="M88.0001 14.3917L93.1501 17.5L91.7834 11.6417L96.3334 7.70002L90.3417 7.19169L88.0001 1.66669L85.6584 7.19169L79.6667 7.70002L84.2167 11.6417L82.8501 17.5L88.0001 14.3917Z"
                  fill="#F3B743"
                />
                <path
                  d="M62 14.3917L67.15 17.5L65.7833 11.6417L70.3333 7.70002L64.3416 7.19169L62 1.66669L59.6583 7.19169L53.6666 7.70002L58.2166 11.6417L56.85 17.5L62 14.3917Z"
                  fill="#F3B743"
                />
                <path
                  d="M36 14.3917L41.15 17.5L39.7833 11.6417L44.3333 7.70002L38.3416 7.19169L36 1.66669L33.6583 7.19169L27.6666 7.70002L32.2166 11.6417L30.85 17.5L36 14.3917Z"
                  fill="#F3B743"
                />
                <path
                  d="M9.99996 14.3917L15.15 17.5L13.7833 11.6417L18.3333 7.70002L12.3416 7.19169L9.99996 1.66669L7.65829 7.19169L1.66663 7.70002L6.21663 11.6417L4.84996 17.5L9.99996 14.3917Z"
                  fill="#F3B743"
                />
                <path
                  d="M114 14.3917L119.15 17.5L117.783 11.6417L122.333 7.70002L116.342 7.19169L114 1.66669L111.658 7.19169L105.667 7.70002L110.217 11.6417L108.85 17.5L114 14.3917Z"
                  fill="#F2F2F2"
                /></svg
            ></label>
            <div>& above</div>
          </div>
          <!-- end star -->

          <!-- star -->
          <div class="flex items-center gap-4">
            <input type="checkbox" name="5" id="5" />
            <label for="5">
              <svg
                width="124"
                height="20"
                viewBox="0 0 124 20"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M88.0001 14.3916L93.1501 17.5L91.7834 11.6416L96.3334 7.69996L90.3417 7.19163L88.0001 1.66663L85.6584 7.19163L79.6667 7.69996L84.2167 11.6416L82.8501 17.5L88.0001 14.3916Z"
                  fill="#F2F2F2"
                />
                <path
                  d="M62 14.3916L67.15 17.5L65.7833 11.6416L70.3333 7.69996L64.3416 7.19163L62 1.66663L59.6583 7.19163L53.6666 7.69996L58.2166 11.6416L56.85 17.5L62 14.3916Z"
                  fill="#F3B743"
                />
                <path
                  d="M36 14.3916L41.15 17.5L39.7833 11.6416L44.3333 7.69996L38.3416 7.19163L36 1.66663L33.6583 7.19163L27.6666 7.69996L32.2166 11.6416L30.85 17.5L36 14.3916Z"
                  fill="#F3B743"
                />
                <path
                  d="M9.99996 14.3916L15.15 17.5L13.7833 11.6416L18.3333 7.69996L12.3416 7.19163L9.99996 1.66663L7.65829 7.19163L1.66663 7.69996L6.21663 11.6416L4.84996 17.5L9.99996 14.3916Z"
                  fill="#F3B743"
                />
                <path
                  d="M114 14.3916L119.15 17.5L117.783 11.6416L122.333 7.69996L116.342 7.19163L114 1.66663L111.658 7.19163L105.667 7.69996L110.217 11.6416L108.85 17.5L114 14.3916Z"
                  fill="#F2F2F2"
                />
              </svg>
            </label>
            <div>& above</div>
          </div>
          <!-- end star -->
          <!-- star -->
          <div class="flex items-center gap-4">
            <input type="checkbox" name="5" id="5" />
            <label for="5">
              <svg
                width="124"
                height="20"
                viewBox="0 0 124 20"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M88.0001 14.3916L93.1501 17.5L91.7834 11.6416L96.3334 7.69996L90.3417 7.19163L88.0001 1.66663L85.6584 7.19163L79.6667 7.69996L84.2167 11.6416L82.8501 17.5L88.0001 14.3916Z"
                  fill="#F2F2F2"
                />
                <path
                  d="M62 14.3916L67.15 17.5L65.7833 11.6416L70.3333 7.69996L64.3416 7.19163L62 1.66663L59.6583 7.19163L53.6666 7.69996L58.2166 11.6416L56.85 17.5L62 14.3916Z"
                  fill="#F2F2F2"
                />
                <path
                  d="M36 14.3916L41.15 17.5L39.7833 11.6416L44.3333 7.69996L38.3416 7.19163L36 1.66663L33.6583 7.19163L27.6666 7.69996L32.2166 11.6416L30.85 17.5L36 14.3916Z"
                  fill="#F3B743"
                />
                <path
                  d="M9.99996 14.3916L15.15 17.5L13.7833 11.6416L18.3333 7.69996L12.3416 7.19163L9.99996 1.66663L7.65829 7.19163L1.66663 7.69996L6.21663 11.6416L4.84996 17.5L9.99996 14.3916Z"
                  fill="#F3B743"
                />
                <path
                  d="M114 14.3916L119.15 17.5L117.783 11.6416L122.333 7.69996L116.342 7.19163L114 1.66663L111.658 7.19163L105.667 7.69996L110.217 11.6416L108.85 17.5L114 14.3916Z"
                  fill="#F2F2F2"
                />
              </svg>
            </label>
            <div>& above</div>
          </div>
          <!-- end star -->
          <!-- star -->
          <div class="flex items-center gap-4">
            <input type="checkbox" name="5" id="5" />
            <label for="5">
              <svg
                width="124"
                height="20"
                viewBox="0 0 124 20"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M88.0001 14.3916L93.1501 17.5L91.7834 11.6416L96.3334 7.69996L90.3417 7.19163L88.0001 1.66663L85.6584 7.19163L79.6667 7.69996L84.2167 11.6416L82.8501 17.5L88.0001 14.3916Z"
                  fill="#F2F2F2"
                />
                <path
                  d="M62 14.3916L67.15 17.5L65.7833 11.6416L70.3333 7.69996L64.3416 7.19163L62 1.66663L59.6583 7.19163L53.6666 7.69996L58.2166 11.6416L56.85 17.5L62 14.3916Z"
                  fill="#F2F2F2"
                />
                <path
                  d="M36 14.3916L41.15 17.5L39.7833 11.6416L44.3333 7.69996L38.3416 7.19163L36 1.66663L33.6583 7.19163L27.6666 7.69996L32.2166 11.6416L30.85 17.5L36 14.3916Z"
                  fill="#F2F2F2"
                />
                <path
                  d="M9.99996 14.3916L15.15 17.5L13.7833 11.6416L18.3333 7.69996L12.3416 7.19163L9.99996 1.66663L7.65829 7.19163L1.66663 7.69996L6.21663 11.6416L4.84996 17.5L9.99996 14.3916Z"
                  fill="#F3B743"
                />
                <path
                  d="M114 14.3916L119.15 17.5L117.783 11.6416L122.333 7.69996L116.342 7.19163L114 1.66663L111.658 7.19163L105.667 7.69996L110.217 11.6416L108.85 17.5L114 14.3916Z"
                  fill="#F2F2F2"
                />
              </svg>
            </label>
            <div>& above</div>
          </div>
          <!-- end star -->
        </div>
        <!-- end stars -->
      </div>
      <!-- rating -->

      <!-- end of rating -->
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
</style>