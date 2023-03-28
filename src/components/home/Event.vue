<script setup>
import Carousel from "@/components/materials/Carousel.vue";
</script>

<template>
  <section id="event" class="pt-28 pb-14 lg:py-16">
    <div class="container">
      <h3
        class="text-xl font-bold text-secondary text-center mb-4 md:text-2xl lg:mt-20"
      >
        Follow new update
      </h3>
      <h1
        class="text-3xl font-bold text-dark text-center mb-4 md:text-5xl lg:mt-3"
      >
        Event
      </h1>
      <p class="text-base text-slate-700 text-center mb-4 md:text-lg lg:mt-3">
        Stay informed about our past events
      </p>
      <div class="w-full justify-center px-4">
        <div
          class="relative mx-auto max-w-lg overflow-hidden rounded-md bg-gray-100 p-2 sm:p-4 mt-9 mb-7"
        >
          <div
            class="absolute top-5 right-0 z-10 rounded-full bg-gray-600 px-2 text-center text-sm text-white"
          ></div>
          <!-- component carousel -->
          <Carousel />
        </div>

        <!-- carousel end -->
      </div>
      <div class="flex flex-wrap justify-center">
        <button
          class="bg-white py-2 px-4 border-2 border-secondary rounded-lg text-secondary my-4 hover:bg-secondary hover:text-white hover:fill-white"
        >
          <p>Read More</p>
        </button>
      </div>
    </div>
  </section>
</template>
