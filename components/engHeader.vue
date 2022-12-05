<template>
  <div id="header" class="">
    <!-- Header NavBar total -->
    <div class="mx-auto w-5/6 pb-2 pt-2 sm:w-full sm:max-w-screen-xl">
      <nav
        id="nav"
        class="flex w-full flex-wrap content-center items-center justify-between py-6"
      >
        <!-- NavBar Logo -->
        <div>
          <nuxt-link to="/eng/"> <Logo class="w-56" /> </nuxt-link>
        </div>
        <!-- Header Hamburger Icon -->
        <div class="block lg:hidden">
          <button
            @click="handleClick"
            class="flex items-center rounded border border-gray-700 px-3 py-2 text-gray-800 hover:border-gray-700 hover:text-gray-700"
          >
            <p class="pr-2 text-xs">MENÜ</p>
            <svg
              class="h-3 w-3 fill-current"
              viewBox="0 0 20 20"
              xmlns="http://www.w3.org/2000/svg"
            >
              <title>Menu</title>
              <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" />
            </svg>
          </button>
        </div>
        <!-- Responsive -->
        <div
          :class="isOpen ? 'block' : 'hidden'"
          class="w-full flex-grow text-center text-gray-800 sm:text-right lg:flex lg:w-auto lg:items-center"
        >
          <div class="lg:flex-grow">
            <!-- NAV Menu Links -->
            <nuxt-link
              class="mt-4 block border-b border-gray-300 px-2 py-2 pb-2 hover:text-gray-900 sm:border-none sm:pb-0 lg:mt-0 lg:inline-block"
              to="/eng/contactform"
              >Contactform</nuxt-link
            >

            <nuxt-link
              class="mt-4 block border-b border-gray-300 px-2 py-2 pb-2 hover:text-gray-900 sm:border-none sm:pb-0 lg:mt-0 lg:inline-block"
              to="/eng/about"
              >About</nuxt-link
            >
            <nuxt-link
              class="mt-4 block border-b border-gray-300 px-2 py-2 pb-2 hover:text-gray-900 sm:border-none sm:pb-0 lg:mt-0 lg:inline-block"
              to="/"
            >
              <FlagGER class="mx-auto w-6" />
            </nuxt-link>
            <nuxt-link
              class="mt-4 block border-b border-gray-300 px-2 py-2 pb-2 hover:text-gray-900 sm:border-none sm:pb-0 lg:mt-0 lg:inline-block"
              to="/eng/"
            >
              <FlagENG class="mx-auto w-7" />
            </nuxt-link>
          </div>
        </div>
      </nav>
    </div>
  </div>
</template>

<script>
import Logo from "./Logo.vue";

export default {
  data() {
    return {
      isOpen: false,
    };
  },
  methods: {
    handleClick() {
      this.isOpen = !this.isOpen;
    },
  },
  components: { Logo },
};
</script>

<style></style>
