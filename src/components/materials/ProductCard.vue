<script setup>
import ProductCarousel from "./ProductCarousel.vue";
// defineProps(["title", "content", "alt", "image"]);
</script>

<template>
  <div class="flex justify-center">
    <div class="block w-full rounded-xl bg-primary shadow-lg">
      <!-- <a href="#!">
        <img class="rounded-t-lg" :src="image" :alt="alt" />
      </a>
      <div class="p-6">
        <h3 class="mb-2 text-xl font-bold leading-tight text-white">
          <a href="#!">{{ title }}</a>
        </h3>
        <p class="mb-4 text-base text-white text-justify">
          {{ content }}
        </p>
      </div> -->
      <ProductCarousel />
    </div>
  </div>
</template>

<Carousel />
