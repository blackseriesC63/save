<template>
  <div class="py-16 px-4 flex flex-col justify-center items-center">
    <h1 class="text-4xl pb-7 text-center">
      Let's build something great <br />
      together
    </h1>

    <div class="text-gray-600 text-center px-4 md:px-12">
      <p>
        We help teams create great digital products by providing them with tools
        and technology <br />
        to make the design-to-code process universally accessible.
      </p>
    </div>

    <div class="flex mt-4 gap-4 flex-wrap justify-center md:flex-row">
      <router-link to="/contact">
        <button
          class="bg-yellow-300 text-black py-2 px-4 rounded-full w-[254px] h-[64px] mx-auto mt-[50px]"
        >
          Contact Us
        </button>
      </router-link>
    </div>
  </div>
</template>

<script setup>
const data = 12;
</script>

<style lang="scss" scoped></style>
