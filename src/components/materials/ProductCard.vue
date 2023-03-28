<script setup>
defineProps(["title", "content", "alt"]);
</script>

<template>
  <div class="flex justify-center">
    <div class="block max-w-sm rounded-lg bg-secondary shadow-lg">
      <a href="#!">
        <img class="rounded-t-lg" src="@/assets/img/product.png" :alt="alt" />
      </a>
      <div class="p-6">
        <h3 class="mb-2 text-xl font-bold leading-tight text-white">
          <a href="#!">{{ title }}</a>
        </h3>
        <p class="mb-4 text-base text-white text-justify">
          {{ content }}
        </p>
      </div>
    </div>
  </div>
</template>
