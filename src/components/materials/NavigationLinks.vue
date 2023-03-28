<script setup></script>

<template>
  <nav
    id="nav-menu"
    class="hidden absolute mt-5 lg:mt-0 py-5 bg-white shadow-lg rounded-lg w-full right-0 top-full lg:block lg:static lg:bg-transparent lg:max-w-full lg:shadow-none lg:rounded-none"
  >
    <ul class="block lg:flex">
      <li class="group">
        <a
          href="#home"
          class="text-base capitalize font-medium text-dark py-3 mx-8 flex group-hover:text-secondary"
          >Home
        </a>
      </li>
      <li class="group">
        <a
          href="#product"
          class="text-base capitalize font-medium text-dark py-3 mx-8 flex group-hover:text-secondary"
          >Product
        </a>
      </li>
      <li class="group">
        <a
          href="#contact"
          class="text-base capitalize font-medium text-dark py-3 mx-8 flex group-hover:text-secondary"
          >Contact
        </a>
      </li>
      <li class="group">
        <a
          href="#about"
          class="text-base capitalize font-medium text-dark py-3 mx-8 flex group-hover:text-secondary"
          >About
        </a>
      </li>
      <li class="group lg:mr-7">
        <a
          href="#event"
          class="text-base capitalize font-medium text-dark py-3 mx-8 flex group-hover:text-secondary"
          >Event
        </a>
      </li>
      <li class="group overflow-hidden flex justify-center">
        <button
          class="w-11/12 lg:w-full my-3 lg:my-0 mx-4 lg:mx-0 bg-secondary rounded-lg hover:opacity-80 transition duration-400 ease-in-out"
        >
          <a
            href="/forum.html"
            class="text-base capitalize font-medium text-white py-3 mx-8 flex justify-center"
            >Forum
          </a>
        </button>
      </li>
    </ul>
  </nav>
</template>
