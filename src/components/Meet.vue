<script setup>
import { ref } from "vue";

const myData = ref([
  {
    name: "John Smith",
    job: "CEO",
    img: [
      "images/facebook.png",
      "images/twitter.png",
      "images/linkedin.png",
      "images/radius.png",
    ],
  },
  {
    name: "Simon Adams",
    job: "CEO",
    img: [
      "images/facebook.png",
      "images/twitter.png",
      "images/linkedin.png",
      "images/radius2.png",
    ],
  },
  {
    name: "Paul Jones",
    job: "Design Lead",
    img: [
      "images/facebook.png",
      "images/twitter.png",
      "images/linkedin.png",
      "images/radius3.png",
    ],
  },
  {
    name: "Sara Hardin",
    job: "Project Manager",
    img: [
      "images/facebook.png",
      "images/twitter.png",
      "images/linkedin.png",
      "images/radius.png",
    ],
  },
]);
</script>

<template>
  <div class="bg-[#F4F6FC]">
    <div class="container mx-auto px-4">
      <div>
        <h2
          class="leading-[40px] md:leading-[64px] text-[28px] md:text-[48px] font-bold text-center mb-[24px] md:mb-[48px] pt-[64px] md:pt-[128px]"
        >
          Meet our team
        </h2>
      </div>
      <div
        class="grid gap-7 md:grid-cols-2 lg:grid-cols-4 pb-[64px] md:pb-[128px] hover:shadow-md"
      >
        <div
          v-for="(item, index) in myData"
          :key="index"
          class="bg-white group hover:shadow-md py-[20px] md:py-[30px] mb-5"
        >
          <div
            class="relative w-[120px] md:w-[168px] h-[120px] md:h-[168px] mx-auto rounded-full overflow-hidden"
          >
            <div
              class="absolute left-0 -bottom-full duration-500 group-hover:bottom-0 w-full h-full bg-violet-500 bg-opacity-50"
            >
              <div class="flex h-full justify-center items-end">
                <div class="flex gap-3 pb-5">
                  <a href="https://www.facebook.com">
                    <img
                      :src="item.img[0]"
                      alt="Facebook"
                      class="w-4 h-4 md:w-4 md:h-4"
                    />
                  </a>
                  <a href="https://x.com">
                    <img
                      :src="item.img[1]"
                      alt="Twitter"
                      class="w-4 h-4 md:w-4 md:h-4"
                    />
                  </a>
                  <a href="https://www.linkedin.com">
                    <img
                      :src="item.img[2]"
                      alt="LinkedIn"
                      class="w-4 h-4 md:w-4 md:h-4"
                    />
                  </a>
                </div>
              </div>
            </div>
            <img :src="item.img[3]" alt="radius" class="w-full h-full" />
          </div>
          <p
            class="text-[18px] md:text-[24px] leading-[28px] md:leading-[36px] font-medium mt-[20px] md:mt-[30px] text-center"
          >
            {{ item.name }}
          </p>
          <p class="text-center text-[14px] md:text-[16px]">{{ item.job }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>
