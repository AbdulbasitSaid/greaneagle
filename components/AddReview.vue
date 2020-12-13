<template>
  <div>
    <div class="w-96 h-screen bg-white flex flex-col p-6">
      <div class="flex items-center gap-2">
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

        <p>Cancel</p>
      </div>

      <div class="p-10 flex flex-col text-sm font-thin gap-6">
        <div>Write a review</div>
        <div>
          Your name
          <input type="text" name="" id="" class="rounded p-2 border w-full" />
        </div>
        <div>
          Your review
          <textarea
            name=""
            id=""
            cols="30"
            rows="5"
            class="rounded border w-full"
          ></textarea>
        </div>
        <div>
          <rating></rating>
        </div>
        <div>
          <input
            type="button"
            value="Submit review"
            class="bg-primary rounded py-2 px-6 text-white"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Rating from "./Rating.vue";
export default {};
</script>

<style lan
Ratingg="scss" scoped>
</style>