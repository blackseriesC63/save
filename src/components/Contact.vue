<template>
  <div class="flex flex-col items-center py-16 px-4 sm:px-6 lg:px-8">
    <div class="text-center">
      <h1 class="text-3xl sm:text-4xl font-bold text-primary">Contact Us</h1>
      <p class="text-gray-500 mt-2 text-base sm:text-lg">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore.
      </p>
    </div>
    <div class="mt-12 bg-gray-50 p-6 sm:p-8 rounded-lg w-full max-w-4xl">
      <form @submit.prevent="submitForm">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
          <div>
            <label class="block text-sm font-medium text-gray-700">Name</label>
            <input
              type="text"
              placeholder="Enter your name"
              class="p-3 sm:p-5 mt-1 block w-full h-12 sm:h-[64px] border-gray-300 rounded-md shadow-sm focus:border-indigo-500 focus:ring-indigo-500"
            />
          </div>
          <div>
            <label class="block text-sm font-medium text-gray-700">Email</label>
            <input
              type="email"
              placeholder="Enter your Email"
              class="p-3 sm:p-5 mt-1 block w-full h-12 sm:h-[64px] border-gray-300 rounded-md shadow-sm focus:border-indigo-500 focus:ring-indigo-500"
            />
          </div>
          <div>
            <label class="block text-sm font-medium text-gray-700"
              >Subject</label
            >
            <input
              type="text"
              placeholder="Provide context"
              class="p-3 sm:p-5 mt-1 block w-full h-12 sm:h-[64px] border-gray-300 rounded-md shadow-sm focus:border-indigo-500 focus:ring-indigo-500"
            />
          </div>
          <div>
            <label class="block text-sm font-medium text-gray-700"
              >Subject</label
            >
            <input
              type="text"
              placeholder="Select Subject"
              class="p-3 sm:p-5 mt-1 block w-full h-12 sm:h-[64px] border-gray-300 rounded-md shadow-sm focus:border-indigo-500 focus:ring-indigo-500"
            />
          </div>
          <div class="md:col-span-2">
            <label class="block text-sm font-medium text-gray-700"
              >Message</label
            >
            <textarea
              rows="4"
              placeholder="Write your question here"
              class="p-3 sm:p-5 mt-1 block w-full h-32 sm:h-[138px] border-gray-300 rounded-md shadow-sm focus:border-indigo-500 focus:ring-indigo-500"
            ></textarea>
          </div>
        </div>
        <div class="mt-6 flex">
          <button
            type="submit"
            class="w-[254px] h-[64px] py-3 bg-black text-white rounded-full shadow-sm hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
          >
            Send Message
          </button>
        </div>
      </form>
    </div>
  </div>
</template>

<script setup>
const submitForm = () => {
  // Handle form submission logic here
  alert("Form submitted!");
};
</script>

<style scoped>
.text-primary {
  color: #333; /* Customize your primary text color */
}
</style>
