<script setup>
import { Carousel, Slide } from "vue3-carousel";

import "vue3-carousel/dist/carousel.css";

const items = [
  {
    id: "1",
    alt: "About - Mitrasoft 1",
    image: "https://iili.io/HPF8Umb.md.jpg",
  },
  {
    id: "2",
    alt: "About - Mitrasoft 2",
    image: "https://iili.io/HPF86LQ.md.jpg",
  },
  {
    id: "3",
    alt: "About - Mitrasoft 3",
    image: "https://iili.io/HPF8LrP.md.jpg",
  },
  {
    id: "4",
    alt: "About - Mitrasoft 4",
    image: "https://iili.io/HPFSfvn.md.jpg",
  },
  {
    id: "5",
    alt: "About - Mitrasoft 5",
    image: "https://iili.io/HPFSoQ4.md.jpg",
  },
];
</script>

<template>
  <Carousel
    :items-to-show="1"
    :wrap-around="true"
    :autoplay="5000"
    :transition="500"
  >
    <Slide v-for="item in items" :key="item.id">
      <div class="carousel__item p-6 lg:mx-4">
        <a href="#!">
          <img
            class="max-w-full mx-auto rounded-xl lg:rounded-3xl shadow-lg"
            :src="item.image"
            :alt="item.alt"
          />
        </a>
      </div>
    </Slide>
  </Carousel>
</template>
