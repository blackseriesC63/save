<template>
  <div class="py-10">
    <div class="container mx-auto px-4">
      <div class="flex justify-center mb-8 flex-wrap gap-2">
        <div class="space-x-2 flex">
          <button
            v-for="category in categories"
            :key="category"
            @click="selectedCategory = category"
            :class="{
              'text-purple-500 bg-slate-50': selectedCategory === category,
              'text-black': selectedCategory !== category,
            }"
            class="px-4 py-2 rounded"
          >
            {{ category }}
          </button>
        </div>
      </div>
      <div
        class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-2 lg:grid-cols-2 gap-8"
      >
        <TemplateCard
          v-for="(template, index) in filteredTemplates"
          :key="index"
          :image="template.image"
          :title="template.title"
          :description="template.description"
          :link="template.link"
        />
      </div>
    </div>
  </div>
</template>

<script>
import TemplateCard from "./TemplateCard.vue";

export default {
  data() {
    return {
      templates: [
        {
          image: "/images/Image.png",
          title: "Template 1",
          description:
            "Apparently we had reached a great height in the atmosphere, for the sky was a dead black, and the stars had ceased to twinkle.",
          link: "#",
          category: "UI Design",
        },
        {
          image: "/images/Image-2.png",
          title: "Template 2",
          description:
            "Apparently we had reached a great height in the atmosphere, for the sky was a dead black, and the stars had ceased to twinkle.",
          link: "#",
          category: "Webflow Design",
        },
        {
          image: "/images/Image-3.png",
          title: "Template 3",
          description:
            "Apparently we had reached a great height in the atmosphere, for the sky was a dead black, and the stars had ceased to twinkle.",
          link: "#",
          category: "Figma Design",
        },
        {
          image: "/images/Image-4.png",
          title: "Template 4",
          description:
            "Apparently we had reached a great height in the atmosphere, for the sky was a dead black, and the stars had ceased to twinkle.",
          link: "#",
          category: "UI Design",
        },
        {
          image: "/images/Image-5.png",
          title: "Template 5",
          description:
            "Apparently we had reached a great height in the atmosphere, for the sky was a dead black, and the stars had ceased to twinkle.",
          link: "#",
          category: "Webflow Design",
        },
        {
          image: "/images/Image-6.png",
          title: "Template 6",
          description:
            "Apparently we had reached a great height in the atmosphere, for the sky was a dead black, and the stars had ceased to twinkle.",
          link: "#",
          category: "Figma Design",
        },
      ],
      categories: ["All", "UI Design", "Webflow Design", "Figma Design"],
      selectedCategory: "All",
    };
  },
  computed: {
    filteredTemplates() {
      if (this.selectedCategory === "All") {
        return this.templates;
      }
      return this.templates.filter(
        (template) => template.category === this.selectedCategory
      );
    },
  },
  components: {
    TemplateCard,
  },
};
</script>

<style scoped>
/* Add any custom styles here */
</style>
