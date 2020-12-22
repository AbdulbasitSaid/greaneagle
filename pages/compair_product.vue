<template>
  <div>
    <main>
      <div class="bg-checkout_bg py-10 px-40">
        <!-- card -->
        <div class="py-6 mx-20 flex flex-col items-center bg-white gap-6">
          <div class="flex justify-start w-full px-12 text-xl">
            Product comparism
          </div>
          <div>
            <table class="table-fixed">
              <thead>
                <tr class="py-4 border-b">
                  <th class="w-64 py-4"></th>
                  <th class="w-64 py-4">
                    <div class="flex justify-end px-6">
                      <svg
                        width="24"
                        height="24"
                        viewBox="0 0 24 24"
                        fill="none"
                        xmlns="http://www.w3.org/2000/svg"
                      >
                        <circle
                          opacity="0.3"
                          cx="12"
                          cy="12"
                          r="10"
                          fill="#2AA580"
                        />
                        <path
                          fill-rule="evenodd"
                          clip-rule="evenodd"
                          d="M16.2782 7.79289C15.8877 7.40237 15.2545 7.40237 14.864 7.79289L12.0355 10.6213L9.20711 7.79289C8.81658 7.40237 8.18342 7.40237 7.79289 7.79289C7.40237 8.18342 7.40237 8.81658 7.79289 9.20711L10.6213 12.0355L7.79289 14.864C7.40237 15.2545 7.40237 15.8877 7.79289 16.2782C8.18342 16.6687 8.81658 16.6687 9.20711 16.2782L12.0355 13.4497L14.864 16.2782C15.2545 16.6687 15.8877 16.6687 16.2782 16.2782C16.6687 15.8877 16.6687 15.2545 16.2782 14.864L13.4497 12.0355L16.2782 9.20711C16.6687 8.81658 16.6687 8.18342 16.2782 7.79289Z"
                          fill="#2AA580"
                        />
                      </svg>
                    </div>
                    <img src="~/assets/images/product1.png" alt="" />
                  </th>
                  <th class="w-64 py-4">
                    <div class="flex justify-end px-6">
                      <svg
                        width="24"
                        height="24"
                        viewBox="0 0 24 24"
                        fill="none"
                        xmlns="http://www.w3.org/2000/svg"
                      >
                        <circle
                          opacity="0.3"
                          cx="12"
                          cy="12"
                          r="10"
                          fill="#2AA580"
                        />
                        <path
                          fill-rule="evenodd"
                          clip-rule="evenodd"
                          d="M16.2782 7.79289C15.8877 7.40237 15.2545 7.40237 14.864 7.79289L12.0355 10.6213L9.20711 7.79289C8.81658 7.40237 8.18342 7.40237 7.79289 7.79289C7.40237 8.18342 7.40237 8.81658 7.79289 9.20711L10.6213 12.0355L7.79289 14.864C7.40237 15.2545 7.40237 15.8877 7.79289 16.2782C8.18342 16.6687 8.81658 16.6687 9.20711 16.2782L12.0355 13.4497L14.864 16.2782C15.2545 16.6687 15.8877 16.6687 16.2782 16.2782C16.6687 15.8877 16.6687 15.2545 16.2782 14.864L13.4497 12.0355L16.2782 9.20711C16.6687 8.81658 16.6687 8.18342 16.2782 7.79289Z"
                          fill="#2AA580"
                        />
                      </svg>
                    </div>
                    <img src="~/assets/images/product4.png" alt="" />
                  </th>
                </tr>
              </thead>
              <tbody>
                <tr class="text-center py-4 border-b">
                  <td class="w-64 py-4">Product Name</td>
                  <td class="w-64 py-4">ARD-6400F</td>
                  <td class="w-64 py-4">73-551-0005i</td>
                </tr>

                <tr class="text-center py-4 border-b font-thin">
                  <td class="w-64 py-4 font-normal">Price</td>
                  <td class="w-64 py-4">$349.00</td>
                  <td class="w-64 py-4">$322.00</td>
                </tr>

                <tr class="text-center py-4 border-b font-thin">
                  <td class="w-64 py-4 font-normal">Model</td>
                  <td class="w-64 py-4">ARD-6400F</td>
                  <td class="w-64 py-4">73-551-0005i</td>
                </tr>
                <tr class="text-center py-4 border-b font-thin">
                  <td class="w-64 py-4 font-normal">Brand</td>
                  <td class="w-64 py-4">Zippy Technology</td>
                  <td class="w-64 py-4">Emerson</td>
                </tr>
                <tr class="text-center py-4 border-b font-thin">
                  <td class="w-64 py-4 font-normal">Availability</td>
                  <td class="w-64 py-4">In Stock</td>
                  <td class="w-64 py-4">In Stock</td>
                </tr>
                <tr class="text-center py-4 border-b font-thin">
                  <td class="w-64 py-4 font-normal">Rating</td>
                  <td class="w-64 py-4">
                    <div class="flex items-center justify-center">
                      <four-stars></four-stars>( 56 )
                    </div>
                  </td>
                  <td class="w-64 py-4">
                    <div class="flex items-center justify-center">
                      <four-stars></four-stars>( 56 )
                    </div>
                  </td>
                </tr>
                <tr class="text-center py-4 border-b font-thin">
                  <td class="w-64 py-4 font-normal">Summary</td>
                  <td class="w-64 py-4">Summary</td>
                  <td class="w-64 py-4">Summary</td>
                </tr>
                <tr class="text-center py-4 border-b font-thin">
                  <td class="w-64 py-4 font-normal">Weight</td>
                  <td class="w-64 py-4">0.00lb</td>
                  <td class="w-64 py-4">0.00lb</td>
                </tr>
                <tr class="text-center py-4 border-b font-thin">
                  <td class="w-64 py-4 font-normal">Dimensions (L x W x H)</td>
                  <td class="w-64 py-4">0.00in x 0.00in x 0.00in</td>
                  <td class="w-64 py-4">0.00in x 0.00in x 0.00in</td>
                </tr>
                <tr class="text-center py-4 font-thin">
                  <td class="w-64 py-4 font-normal"></td>
                  <td class="w-64 py-4">
                    <div>
                      <input
                        type="button"
                        value="Add to Cart"
                        class="rounded bg-white border py-2 px-4"
                      />
                    </div>
                  </td>
                  <td class="w-64 py-4">
                    <div>
                      <input
                        type="button"
                        value="Add to Cart"
                        class="rounded bg-white border py-2 px-4"
                      />
                    </div>
                  </td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
        <!-- card -->
      </div>
    </main>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
</style>