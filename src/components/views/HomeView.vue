<script setup>
import NavigationBar from "@/components/materials/NavigationBar.vue";
import Hero from "@/components/home/Hero.vue";
import Profile from "@/components/home/Profile.vue";
import Product from "@/components/home/Product.vue";
import Contact from "@/components/home/Contact.vue";
import About from "@/components/home/About.vue";
// import Event from "@/components/home/Event.vue";
import Partner from "../home/Partner.vue";
import Client from "@/components/home/Client.vue";
import Footer from "@/components/materials/Footer.vue";
</script>

<template>
  <main>
    <NavigationBar />
    <Hero />
    <Profile />
    <Product />
    <Contact />
    <About />
    <!-- <Event /> -->
    <Partner />
    <Client />
    <Footer />
  </main>
</template>
