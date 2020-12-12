<template>
  <div>
    <div class="flex justify-center items-center py-20">
      <div class="flex-col w-80">
        <product-list-title>Returning Customer</product-list-title>
        <!-- form -->
        <div class="space-y-4">
          <div class="text-sm font-thin">
            You don’t have an account yet ?
            <nuxt-link to="register" class="text-primary font-bold">
              Create Account</nuxt-link
            >
          </div>
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
          <div>
            <nuxt-link to="reset_password" class="underline text-sm font-thin">
              I forgot my password
            </nuxt-link>
          </div>
          <div>
            <nuxt-link
              to="account_success"
              class="bg-primary py-2 px-6 rounded text-white"
              >Submit</nuxt-link
            >
          </div>
        </div>
        <!-- end form -->
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
</style>