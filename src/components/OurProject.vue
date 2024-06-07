<template>
  <div class="container mx-auto px-4 pb-32">
    <h1 class="text-[#282938] text-2xl md:text-4xl font-bold mt-14 mb-16">
      View our projects
    </h1>

    <div class="grid grid-cols-1 md:grid-cols-3 gap-5">
      <div class="md:col-span-2 md:row-span-2 relative group overflow-hidden">
        <div
          class="h-full group-hover:left-0 w-[50%] duration-300 -left-full top-0 absolute bg-gradient-to-r from-[#1C1E536B]/40 to-[#1C1E53]"
        >
          <div
            class="absolute inset-0 flex flex-col justify-center items-center p-10"
          >
            <h1
              class="text-xl md:text-2xl font-bold text-[#FFFFFF] text-center"
            >
              Workhub office Webflow Webflow Design
            </h1>
            <p
              class="mt-4 mb-4 text-sm md:text-base font-normal text-[#FFFFFF] text-center"
            >
              Euismod faucibus turpis eu gravida mi. Pellentesque et velit
              aliquam
            </p>
            <div class="flex gap-5 items-center justify-center">
              <p class="text-base leading-7 font-medium text-[#FCD980]">
                View project
              </p>
              <img class="w-6 h-2.5 rounded-sm" src="/images/Arrow.png" />
            </div>
          </div>
        </div>
        <img class="w-full h-full object-cover" src="/images/Card.png" />
      </div>
      <div class="relative overflow-hidden group">
        <div
          class="h-full group-hover:left-0 w-[50%] duration-300 -left-full top-0 absolute bg-gradient-to-r from-[#1C1E536B]/40 to-[#1C1E53] p-10 flex flex-col justify-center items-center"
        >
          <h1 class="text-xl md:text-2xl font-bold text-white text-center">
            Unisaas Website
          </h1>
          <p
            class="mt-4 mb-4 text-sm md:text-base font-normal text-[#FFFFFF] text-center"
          >
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod,
            cumque?
          </p>
        </div>
        <img class="w-full h-full object-cover" src="/images/1.png" />
      </div>
      <div>
        <img class="w-full h-full object-cover" src="/images/2.png" />
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.group:hover .group-hover\:left-0 {
  left: 0;
}

.group-hover\:left-0 {
  left: -100%;
}

@media (max-width: 768px) {
  .group-hover\:left-0 {
    left: -100%;
    position: absolute;
    width: 100%;
    height: 100%;
  }

  .group:hover .group-hover\:left-0 {
    left: 0;
  }
}
</style>
