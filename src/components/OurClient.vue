<template>
  <div class="bg-white py-6 md:py-[106px]">
    <div class="container mx-auto px-4">
      <div class="md:grid md:grid-cols-3">
        <div class="mb-6 md:mb-0">
          <h2 class="text-[#282938] font-bold text-2xl md:text-3xl mb-3">
            What our clients say about us
          </h2>
          <p class="text-base">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit sed.
          </p>
        </div>
        <div class="md:col-span-2">
          <h2 class="text-[#282938] font-medium text-lg md:text-2xl mb-3  pl-5">
            "{{ reviews[currentReview].quote }}"
          </h2>
          <div class="flex items-center gap-4 mt-6 md:mt-0 justify-between  pl-5">
            <div class="flex items-center gap-3 pt-2">
              <img
                :src="reviews[currentReview].image"
                class="rounded-full w-16 h-16 md:w-24 md:h-24"
              />
              <div>
                <p class="text-lg font-bold">
                  {{ reviews[currentReview].name }}
                </p>
                <p class="text-[#282938] text-sm">
                  {{ reviews[currentReview].title }}
                </p>
              </div>
            </div>
            <div class="flex gap-4 mt-6">
              <button
                @click="prevReview"
                class="border border-black px-4 py-2 rounded-full focus:bg-blue-600"
              >
                <
              </button>
              <button
                @click="nextReview"
                class="border border-black px-4 py-2 rounded-full focus:bg-blue-600"
              >
                >
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const reviews = ref([
  {
    quote:
      "The best agency we’ve worked with so far. new features with a great focus.",
    image: "/images/radius.png",
    name: "Jenny Wilson",
    title: "Vice President",
  },
  {
    quote: "A fantastic team! They always deliver quality work on time.",
    image: "/images/radius2.png",
    name: "John Doe",
    title: "CEO",
  },
  {
    quote:
      "Their attention to detail and dedication to the project was impressive.",
    image: "/images/radius3.png",
    name: "Sara Smith",
    title: "Project Manager",
  },
  {
    quote:
      "Their attention to detail and dedication to the project was impressive.",
    image: "/images/woman.jpg",
    name: "Sara Smith",
    title: "Project Manager",
  },
]);

const currentReview = ref(0);

const prevReview = () => {
  currentReview.value =
    (currentReview.value - 1 + reviews.value.length) % reviews.value.length;
};

const nextReview = () => {
  currentReview.value = (currentReview.value + 1) % reviews.value.length;
};
</script>

<style lang="scss" scoped></style>
