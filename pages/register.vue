<template>
  <div>
    <div class="flex justify-center items-center py-20">
      <div class="flex-col w-80">
        <product-list-title>Register Account</product-list-title>
        <!-- form -->
        <div class="space-y-4">
          <div class="text-sm font-thin">
            If you already have an account with us
            <nuxt-link to="login" class="text-primary font-bold">
              Login</nuxt-link
            >
          </div>
          <!-- name -->
          <div class="grid grid-cols-2 text-sm font-thin gap-6">
            <div>
              Title
              <input
                type="text"
                name=""
                id=""
                class="border p-2 rounded"
                placeholder="Mr."
              />
            </div>
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
              Middle name
              <input
                type="text"
                name=""
                id=""
                class="border p-2 rounded"
                placeholder="Said"
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

          <!-- Interest -->
          <div class="text-sm font-thin">
            <div class="flex flex-col">
              Interest
              <input
                type="text"
                name=""
                id=""
                class="border p-2 rounded w-full block"
                placeholder="Select Interest"
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

          <!-- Password -->
          <div class="text-sm font-thin">
            <div class="flex flex-col">
              Password
              <input
                type="text"
                name=""
                id=""
                class="border p-2 rounded w-full block"
                placeholder="minimum of 8 characters"
              />
            </div>
          </div>
          <!-- end -->

          <!-- Confirm Password -->
          <div class="text-sm font-thin">
            <div class="flex flex-col">
              Confirm password
              <input
                type="text"
                name=""
                id=""
                class="border p-2 rounded w-full block"
                placeholder="Confirm your password"
              />
            </div>
          </div>
          <!-- end -->

          <!-- news teller request -->
          <div class="text-sm font-thin">
            Do you want to subscribe for newsletter ?
            <!-- yes no -->
            <div>
              <input type="checkbox" name="yes" id="yes" />
              <label for="yes">yes</label>
            </div>
            <!-- end -->
          </div>
          <!-- end -->
        </div>
        <!-- end form -->
      </div>
    </div>
    <subscribe-now></subscribe-now>
  </div>
</template>

<script>
import ProductListTitle from "../components/ProductListTitle.vue";
export default {
  components: { ProductListTitle },
};
</script>

<style lang="scss" scoped>
</style>