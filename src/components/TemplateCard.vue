<template lang="">
  <div class="bg-white rounded-lg overflow-hidden pr-3">
    <img :src="image" alt="Template Image" class="w-full object-cover" />
    <div class="p-4">
      <h2 class="text-xl font-bold">{{ title }}</h2>
      <p class="text-gray-600 mt-2">{{ description }}</p>
      <a :href="link" class="mt-4 block">Read case study &rarr;</a>
    </div>
  </div>
</template>
<script>
export default {
  props: ["image", "title", "description", "link"],
};
</script>
<style lang=""></style>
