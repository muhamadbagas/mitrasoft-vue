<script setup>
import ProductCard from "../materials/ProductCard.vue";
</script>

<template>
  <section id="product" class="pt-28 pb-8 lg:py-16">
    <div class="container">
      <h3
        class="text-xl font-bold text-secondary text-center mb-4 md:text-2xl lg:mt-20"
      >
        Get what you need
      </h3>
      <h1
        class="text-3xl font-bold text-dark text-center mb-4 md:text-5xl lg:mt-3"
      >
        Product
      </h1>
      <p
        class="text-base text-slate-700 text-justify lg:text-center mb-4 px-4 md:px-24 md:text-lg lg:mt-3"
      >
        Our product give the powerful features and ease of use, it's perfect for
        your sharia banking business. Plus, our professional team are always
        available to provide you with outstanding support and service.
      </p>

      <div class="flex flex-wrap mt-12">
        <div class="w-full">
          <ProductCard />
        </div>

        <!-- <div class="w-full self-center px-4 lg:w-1/3">
          <ProductCard
            title="CBS Islamic Banking Application (IBA)"
            content="CBS Islamic Banking Application (IBA) system is
                    customizable, integrates easily with other systems, and
                    provides real-time processing and reporting capabilities."
            alt="Islamic Banking Application"
            image="https://iili.io/H6BQ2hG.md.png"
          />
        </div>
        <div class="w-full self-center px-4 my-9 lg:my-0 lg:w-1/3">
          <ProductCard
            title="CBS Islamic Micro Finance Application (IMFA)"
            content="CBS Islamic Micro Finance Application (IMFA) system is
                    designed to focus on providing financial services to
                    low-income communities and promoting financial inclusion."
            alt="Islamic Micro Finance Application"
            image="https://iili.io/H6CCXbs.png"
          />
        </div>
        <div class="w-full self-start px-4 lg:w-1/3">
          <ProductCard
            title="Education Application (EDA)"
            content="Education Application (EDA) is a reliable and user-friendly
                    solution for educational institutions, offering features and
                    capabilities to support their daily operations and enhance
                    the learning experience."
            alt="Education Application"
            image="https://iili.io/H63KWyN.png"
          />
        </div> -->
      </div>
    </div>
  </section>
</template>
