<template>
  <div>
    <div class="container pt-24 sm:pt-32 md:pt-40 lg:pt-52">
      <h1
        class="text-[28px] sm:text-[36px] md:text-[44px] lg:text-[50px] font-bold leading-[36px] sm:leading-[44px] md:leading-[54px] lg:leading-[64px] text-center text-primary w-full sm:w-[600px] md:w-[700px] lg:w-[825px] mx-auto"
      >
        A UX Case Study on Creating a Studious Environment for Students
      </h1>
      <p
        class="text-[16px] sm:text-[18px] font-semibold leading-[24px] sm:leading-[28px] text-center text-primary mb-6 sm:mb-8 md:mb-10 mt-4 sm:mt-6"
      >
        Posted on 27th January 2021
      </p>
      <img class="w-full h-auto" src="../../public/images/blog1.png" alt="" />
      <p
        class="text-[16px] sm:text-[18px] leading-[24px] sm:leading-[28px] text-center text-primary mt-6 sm:mt-8 md:mt-10 mb-4 sm:mb-6 md:mb-8 w-full sm:w-[600px] md:w-[700px] lg:w-[825px] mx-auto"
      >
        Apparently we had reached a great height in the atmosphere, for the sky
        was a dead black, and the stars had ceased to twinkle. By the same
        illusion which lifts the horizon of the sea to the level of the
        spectator on a hillside.
      </p>
      <button
        class="text-[#2405F2] text-center w-full text-[16px] sm:text-[18px] leading-[24px] sm:leading-[28px] mb-10 sm:mb-16 md:mb-24"
      >
        Read more
      </button>
      <h2
        class="text-[28px] sm:text-[36px] md:text-[44px] lg:text-[50px] leading-[36px] sm:leading-[44px] md:leading-[54px] lg:leading-[64px] font-bold text-center text-primary mb-8 sm:mb-10"
      >
        Our Blog
      </h2>
      <div
        class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-x-4 sm:gap-x-6 md:gap-x-10 gap-y-8 sm:gap-y-12 md:gap-y-14 mb-10 sm:mb-16 md:mb-20"
      >
        <template v-for="item in gridDatas" :key="item.id">
          <BlogGrid :item="item" />
        </template>
      </div>
    </div>
  </div>
</template>

<script setup>
import BlogGrid from "./BlogGrid.vue";

const gridDatas = [
  {
    id: 1,
    img: "images/blogGrid.png",
    data: "27 Jan 2021",
    text: "How one Webflow user grew his single person consultancy from $0-100K in 14 months",
    content:
      "See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract",
  },
  {
    id: 2,
    img: "images/blogGrid1.png",
    data: "27 Jan 2021",
    text: "How one Webflow user grew his single person consultancy from $0-100K in 14 months",
    content:
      "See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract",
  },
  {
    id: 3,
    img: "images/blogGrid2.png",
    data: "27 Jan 2021",
    text: "How one Webflow user grew his single person consultancy from $0-100K in 14 months",
    content:
      "See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract",
  },
  {
    id: 4,
    img: "images/blogGrid3.png",
    data: "27 Jan 2021",
    text: "How one Webflow user grew his single person consultancy from $0-100K in 14 months",
    content:
      "See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract",
  },
  {
    id: 5,
    img: "images/blogGrid2.png",
    data: "27 Jan 2021",
    text: "How one Webflow user grew his single person consultancy from $0-100K in 14 months",
    content:
      "See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract",
  },
  {
    id: 6,
    img: "images/blogGrid5.png",
    data: "27 Jan 2021",
    text: "How one Webflow user grew his single person consultancy from $0-100K in 14 months",
    content:
      "See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract",
  },
];
</script>

<style lang="scss" scoped></style>
