<template>
  <div class="container mx-auto px-4">
    <div class="md:grid grid-cols-2 pt-12 pb-2 gap-4">
      <div class="w-full md:w-[595px]">
        <h2 class="text-lg font-normal mb-2">About us</h2>
        <h2
          class="text-2xl md:text-5xl font-bold leading-tight md:leading-[77px] mb-8"
        >
          Our designs solve problems
        </h2>
        <p class="mb-4 mt-4 leading-7 text-base md:text-lg font-normal">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad
          minim veniam.
        </p>
      </div>
      <div class="flex justify-center">
        <img src="/images/about.png" class="w-full max-w-md md:max-w-full" />
      </div>
    </div>
  </div>
</template>

<script setup>
const data = 12;
</script>

<style lang="scss" scoped>
.container {
  @apply max-w-screen-lg;
}
</style>
