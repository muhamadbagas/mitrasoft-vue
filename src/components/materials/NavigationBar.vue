<script setup>
import { onMounted } from "vue";

import LogoPrimary from "./LogoPrimary.vue";
import NavigationLinks from "./NavigationLinks.vue";
import NavigationMobile from "./NavigationMobile.vue";

onMounted(() => {
  // Fixed Navbar
  window.onscroll = function () {
    const header = document.querySelector("header");
    const fixedNav = header.offsetTop;

    if (window.scrollY > fixedNav) {
      header.classList.add("navbar-fixed");
    } else {
      header.classList.remove("navbar-fixed");
    }
  };

  // Hamburger Menu
  const hamburger = document.querySelector("#hamburger");
  const navMenu = document.querySelector("#nav-menu");

  hamburger.addEventListener("click", function () {
    hamburger.classList.toggle("hamburger-active");
    navMenu.classList.toggle("hidden");
  });
});
</script>

<template>
  <header class="absolute top-0 left-0 w-full flex items-center z-10">
    <div class="container lg:px-0 mb-5 lg:mb-0">
      <div class="flex items-center justify-between relative mt-5 lg:mt-0">
        <LogoPrimary />
        <div class="flex items-center px-4">
          <NavigationMobile />
          <NavigationLinks />
        </div>
      </div>
    </div>
  </header>
</template>
