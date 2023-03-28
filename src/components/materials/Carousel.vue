<script setup>
import { Carousel, Navigation, Slide } from "vue3-carousel";
import "vue3-carousel/dist/carousel.css";

const items = [
  {
    id: "1",
    src: "https://iili.io/HN8G1GR.jpg",
  },
  {
    id: "2",
    src: "https://iili.io/HN8Gjun.jpg",
  },
  {
    id: "3",
    src: "https://iili.io/HN8GYTg.jpg",
  },
  {
    id: "4",
    src: "https://iili.io/HN8GXyX.jpg",
  },
  {
    id: "5",
    src: "https://iili.io/HN8GM3N.jpg",
  },
];
</script>

<template>
  <Carousel :items-to-show="1" :wrap-around="true">
    <Slide v-for="item in items" :key="item.id">
      <div class="carousel__item">
        <img :src="item.src" alt="event" />
      </div>
    </Slide>

    <template #addons>
      <Navigation />
    </template>
  </Carousel>
</template>
