<template>
  <div>
    <div class="flex justify-center items-center py-20">
      <div class="flex-col w-80">
        <product-list-title>Reset your password</product-list-title>
        <!-- form -->
        <div class="space-y-4">
          <div class="text-sm font-thin">
            Enter your email and we will send you a link to reset your password.
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

          <div
            class="text-center bg-primary py-2 px-4 text-white rounded my-10"
          >
            Send Instructions
          </div>
          <div class="text-center">
            I remember my password
            <nuxt-link to="login" class="text-primary">Try Login</nuxt-link>
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