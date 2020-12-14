<template>
  <div class="bg-white w-96">
    <div class="min-h-screen border-r py-6 pl-10 pr-4 flex flex-col gap-6">
      <!--  -->
      <div class="flex border-b space-x">
        <nuxt-link to="/" class="px-3 py-4">Request Quote</nuxt-link>
      </div>
      <!--  -->
      <!-- product name -->
      <div class="text-sm font-thin">
        <div class="flex flex-col">
          Product name
          <input
            type="text"
            name=""
            id=""
            class="border p-2 rounded w-full block bg-white"
            value="V07106"
            disabled
            placeholder="Select Interest"
          />
        </div>
      </div>
      <!-- end -->
      <div class="flex justify-center items-center text-sm font-thin gap-2">
        <div>
          Quantity required
          <input
            type="number"
            name=""
            id=""
            value="1"
            class="border p-2 rounded"
            placeholder=""
          />
        </div>
        <div>
          Condition
          <input
            type="text"
            name=""
            id=""
            value="Refurbished"
            class="border p-2 rounded"
            placeholder="Refurbished"
          />
        </div>
      </div>
      <!--  -->
      <div class="pb-10">
        Comment
        <textarea
          name=""
          id=""
          cols="30"
          rows="5"
          class="rounded border w-full"
        ></textarea>
      </div>
      <!--  -->
      <hr />
      <div class="text-lg">Personal Information</div>
      <p>Please fill in your details, and we promise to get back to you</p>
      <!-- name -->
      <div class="grid grid-cols-2 text-sm font-thin gap-2">
        <div>
          First name
          <input
            type="text"
            name=""
            id=""
            class="border p-2 rounded"
            placeholder="Abdulbasit"
          />
        </div>

        <div>
          Last name
          <input
            type="text"
            name=""
            id=""
            class="border p-2 rounded"
            placeholder="Ibrahim"
          />
        </div>
      </div>
      <!-- end -->
      <!-- email adderess -->
      <div class="text-sm font-thin">
        <div class="flex flex-col">
          Email address
          <input
            type="text"
            name=""
            id=""
            class="border p-2 rounded w-full block"
            placeholder="abdulbasitsaeed619@gmail.com"
          />
        </div>
      </div>
      <!-- end -->
      <!-- phone number -->
      <div class="text-sm font-thin">
        <div class="flex flex-col">
          Phone Number
          <div class="flex gap-2">
            <select name="cars" id="cars" class="focus:border-gray-600">
              <option value="ng">+234</option>
              <option value="us">+244</option>
              <option value="uk">+344</option>
              <option value="cn">+999</option>
            </select>
            <input
              type="text"
              name=""
              id=""
              class="border p-2 rounded w-full block"
              placeholder="08108817419"
            />
          </div>
        </div>
      </div>
      <!-- end -->
      <!-- Interest -->
      <div class="text-sm font-thin">
        <div class="flex flex-col">
          Enterprise
          <input
            type="text"
            name=""
            id=""
            class="border p-2 rounded w-full block"
            placeholder=""
          />
        </div>
      </div>
      <!-- end -->
      <div class="flex gap-2">
        <div class="flex gap-2 items-center">
          <svg
            width="15"
            height="15"
            viewBox="0 0 15 15"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              opacity="0.3"
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M11.25 8.125C11.5952 8.125 11.875 7.84518 11.875 7.5C11.875 7.15482 11.5952 6.875 11.25 6.875H3.75C3.40482 6.875 3.125 7.15482 3.125 7.5C3.125 7.84518 3.40482 8.125 3.75 8.125H11.25Z"
              fill="#2AA580"
            />
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M7.94194 10.8081C8.18602 11.0521 8.18602 11.4479 7.94194 11.6919C7.69787 11.936 7.30214 11.936 7.05806 11.6919L3.30806 7.94194C3.07145 7.70533 3.06317 7.32434 3.28928 7.07767L6.72678 3.32767C6.96002 3.07322 7.35538 3.05603 7.60983 3.28928C7.86428 3.52252 7.88147 3.91788 7.64822 4.17233L4.61509 7.4812L7.94194 10.8081Z"
              fill="#2AA580"
            />
          </svg>
          <nuxt-link to="product_detail"> Back to shopping </nuxt-link>
        </div>
        <div><primary-button-rounded>Send request</primary-button-rounded></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
</style>