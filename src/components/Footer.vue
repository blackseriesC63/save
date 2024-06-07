<script setup>
import { reactive } from "vue";
</script>

<template>
  <div class="bg-[#1C1E53] py-10 md:py-[100px]">
    <div class="container mx-auto px-4">
      <div class="grid gap-10 md:grid-cols-2 items-center">
        <div>
          <img src="/images/Logo.png" alt="Logo" />
          <p class="text-white mt-4">
            We are always open to discuss your project and improve your online
            presence
          </p>
          <div class="bg-[#FCD980] text-[#282938] py-4 px-6 mt-6 md:mt-20">
            <div class="mb-4 md:mb-0">
              <p class="text-lg md:text-xl font-bold">
                <a href="https://www.google.com/intl/ru/gmail/about/"
                  >Email me at</a
                >
              </p>
              <p>nizomiddinazam@gmail.com</p>
            </div>
            <div>
              <p class="text-lg md:text-xl font-bold">Call us</p>
              <p>+99897-949-91-90</p>
            </div>
          </div>
        </div>
        <div>
          <h1 class="text-3xl md:text-4xl font-bold text-white">Let's Talk!</h1>
          <p class="mt-4 text-white">
            We are always open to discuss your project, improve your online
            presence, and help with your UX/UI design challenges.
          </p>
          <div class="flex mt-4 gap-4">
            <div class="flex gap-x-[27px] justify-center">
              <a href="https://www.facebook.com/">
                <img src="../../public/images/facebook.png" />
              </a>
              <a href="https://x.com/?lang=en">
                <img src="../../public/images/instragram.png" />
              </a>
              <a href="https://www.instagram.com/">
                <img src="../../public/images/twitter.png" />
              </a>
              <a href="https://uz.linkedin.com/">
                <img src="../../public/images/linkedin.png" />
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>
