<template>
  <div>
    <section class="bg-[#1C1E53] py-[128px]">
      <div class="container">
        <div class="max-md:flex-col md:flex gap-x-8 items-center">
          <!-- Added items-center -->
          <div class="">
            <h1
              class="mb-7 text-[25px] md:text-[54px] max-w-[500px] mx-auto md:max-w-[582px] text-[white] font-bold leading-[42px] md:leading-[74px]"
            >
              Building stellar websites for early startups
            </h1>
            <p
              class="max-md:max-w-[500px] max-md:mx-auto max-w-[460px] font-medium text-[16px] leading-7 text-[white]"
            >
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt.
            </p>
            <div
              class="max-md:mb-[50px] flex gap-x-[55px] mt-[50px] items-center"
            >
              <router-link to="/work">
                <button
                  class="max-md:ml-4 rounded-3xl font-medium border border-white-500 py-3 px-8 md:py-4 md:px-16 bg-[#FCD980]"
                >
                  View our work
                </button>
              </router-link>
              <div class=" ">
                <router-link to="/pricing">
                  <p
                    class="max-md:pb-2 text-3 mt-2 md:text-[14px] font-medium leading-7 text-[white] cursor-pointer"
                  >
                    View Pricing
                  </p>
                </router-link>
              </div>
            </div>
          </div>
          <div class="max-md:mt-10">
            <!-- Added margin top for spacing -->
            <img
              class="max-w-full max-md:w-[60%] mx-auto"
              src="/images/intro.png"
            />
            <!-- Centered the image using mx-auto -->
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
