<template>
  <div
    class="flex flex-col md:flex-row justify-between items-start mx-auto p-6 rounded-lg w-[1280px] h-[562px]"
  >
    <div class="w-full md:w-1/3">
      <h2 class="text-4xl font-bold mb-2">Frequently asked questions</h2>
      <a href="#" class="text-purple-600">Contact us For More Info</a>
    </div>
    <div class="w-full md:w-2/3 text-left">
      <div
        v-for="(item, index) in faqItems"
        :key="index"
        class="faq-item border-b py-4 pt-[32px]"
      >
        <div
          @click="toggle(index)"
          class="faq-question flex justify-between items-center cursor-pointer"
        >
          <div class="items-center flex">
            <span class="font-bold text-purple-600 mr-2">{{
              String(index + 1).padStart(2, "0")
            }}</span>
            <span>{{ item.question }}</span>
          </div>
          <div>
            <span
              v-if="activeIndex === index"
              class="text-purple-600 cursor-pointer"
              >✕</span
            >
            <span v-else class="text-purple-600 cursor-pointer">+</span>
          </div>
        </div>
        <div v-if="activeIndex === index" class="faq-answer py-4">
          <p>{{ item.answer }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      activeIndex: null,
      faqItems: [
        {
          question: "How much time does it take ?",
          answer:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
        },
        {
          question: "What is your class naming convention ?",
          answer: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
        },
        {
          question: "How do we communicate ?",
          answer: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
        },
        {
          question: "I have a bigger project. Can you handle it ?",
          answer: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
        },
        {
          question: "What is your class naming convention ?",
          answer: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
        },
      ],
    };
  },
  methods: {
    toggle(index) {
      if (this.activeIndex === index) {
        this.activeIndex = null;
      } else {
        this.activeIndex = index;
      }
    },
  },
};
</script>

<style scoped>
.faq-item {
  transition: all 0.3s ease;
}

@media (max-width: 768px) {
  /* Styles for mobile devices */
  .faq-question {
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
  }
  .faq-question span:first-child {
    margin-bottom: 8px;
  }
  .flex {
    /* Remove fixed width/height on mobile */
    width: auto;
    height: auto;
  }
}
</style>
