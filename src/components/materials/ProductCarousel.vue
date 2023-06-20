<script setup>
import { defineComponent } from "vue";
import { Carousel, Navigation, Slide } from "vue3-carousel";

import "vue3-carousel/dist/carousel.css";

const responsiveBreakpoints = defineComponent({
  name: "breakpoints",
  components: {
    Carousel,
    Slide,
    Navigation,
  },
  data: () => ({}),
});

const items = [
  {
    id: "1",
    title: "CBS Islamic Banking Application (IBA)",
    content:
      "CBS Islamic Banking Application (IBA) system is customizable, integrates easily with other systems, and provides real-time financial processing and reporting capabilities.",
    alt: "Islamic Banking Application",
    image: "https://iili.io/H6BQ2hG.md.png",
  },
  {
    id: "2",
    title: "CBS Islamic Micro Finance Application (IMFA)",
    content:
      "CBS Islamic Micro Finance Application (IMFA) system is designed to focus on providing financial services to low-income communities and promoting financial inclusion.",
    alt: "Islamic Micro Finance Application",
    image: "https://iili.io/H6CCXbs.png",
  },
  {
    id: "3",
    title: "Education Application (EDA)",
    content:
      "Education Application (EDA) is a reliable and user-friendly desktop application solution for educational institutions. We provide any features to support and manage your financial operations in educational institution.",
    alt: "Education Application",
    image: "https://iili.io/H6AoSgn.png",
  },
  {
    id: "4",
    title: "Mini Bank",
    content:
      "Mini Bank is a small scale financial institution that operates within the school or university. We provide and support Mini Bank with banking application to help Mini Bank operates and run their own Banking Services.",
    alt: "Mini Bank",
    image: "https://iili.io/H6AIizv.png",
  },
  {
    id: "5",
    title: "IBA/IMFA Mobile Application",
    content:
      "Islamic Banking Application (IBA) / Islamic Micro Finance Application (IMFA) Mobile Application is a Banking Application in a mobile version that we provides real-time processing and reporting capabilities on mobile banking services.",
    alt: "IBA/IMFA Mobile Application",
    image: "https://iili.io/H6BQ2hG.md.png",
  },
  {
    id: "6",
    title: "Virtual Account",
    content:
      "We provide virtual account number in order to help BPRS to receive any transfer of funds from another bank into BPRS Bank Account. With our innovative virtual account product, users can connected to their funds with ease and convenience.",
    alt: "Virtual Account",
    image: "https://iili.io/H6AaFwX.png",
  },
  {
    id: "7",
    title: "Transfer Out",
    content:
      "We provide Transfer Out service in order to help BPRS to transfer any funds from BPRS Bank Account to another bank. Our Transfer Out product streamlines the process of sending funds securely and swiftly to any destination.",
    alt: "Transfer Out",
    image: "https://iili.io/H6AjYVp.png",
  },
  {
    id: "8",
    title: "Mobile Collector",
    content:
      "We provide Mobile Collector service in order to help BPRS collecting their fund from the debtor. With our Mobile Collector, managing and resolving debts become a seamless and efficient process just with your mobile collector device.",
    alt: "Mobile Collector",
    image: "https://iili.io/H6w0GI4.png",
  },
  {
    id: "9",
    title: "Cloud Server",
    content:
      "We provide and maintaining cloud server for BPRS to running their banking application server needs. With our robust cloud server product, we provide a scalable and secure infrastructure that empowers you to effortlessly manage the server.",
    alt: "Cloud Server",
    image: "https://iili.io/H6pGhTQ.png",
    // https://iili.io/H6AvS5P.png
  },
  {
    id: "10",
    title: "SMS Masking",
    content:
      "We provide SMS Masking to make your SMS broadcast more professional by masking the sender number into your business name on a customer contact, enhances your business's reputation and builds trust.",
    alt: "SMS Masking",
    image: "https://iili.io/H6EjD4n.png",
  },
  {
    id: "11",
    title: "Payment Point Online Bank (PPOB)",
    content:
      "We provide Payment Point Online Bank (PPOB) for additional features banking application with PPOB payment services to make a payment for BPJS, PLN, PDAM, E-Wallet, etc.",
    alt: "PPOB",
    image: "https://iili.io/H6EV4x1.png",
  },
];
</script>

<template>
  <!-- Carousel Large Display -->
  <div class="hidden lg:block">
    <Carousel :items-to-show="3" :wrap-around="true" :transition="500">
      <Slide v-for="item in items" :key="item.id">
        <div class="carousel__item p-6 mx-4">
          <a href="#!">
            <img class="rounded-t-lg" :src="item.image" :alt="item.alt" />
          </a>
          <div class="p-6">
            <h3 class="mb-2 text-xl font-bold leading-tight text-white">
              <a href="#!">{{ item.title }}</a>
            </h3>
            <p class="mb-4 text-base text-white text-justify-content">
              {{ item.content }}
            </p>
          </div>
        </div>
      </Slide>

      <template #addons>
        <Navigation />
      </template>
    </Carousel>
  </div>

  <!-- Carousel Small Display -->
  <div class="block lg:hidden">
    <Carousel
      :items-to-show="1"
      :wrap-around="true"
      :transition="500"
      :autoplay="8000"
    >
      <Slide v-for="item in items" :key="item.id">
        <div class="carousel__item p-4 mx-4">
          <a href="#!">
            <img
              class="justify-centers rounded-t-lg"
              :src="item.image"
              :alt="item.alt"
            />
          </a>
          <div class="p-6">
            <h3 class="mb-2 text-xl font-bold leading-tight text-white">
              <a href="#!">{{ item.title }}</a>
            </h3>
            <p class="mb-1 text-base text-white text-justify-content">
              {{ item.content }}
            </p>
          </div>
        </div>
      </Slide>

      <template #addons>
        <Navigation class="text-white" />
      </template>
    </Carousel>
  </div>
</template>
