<template>
  <nav class="relative container mx-auto p-6">
    <div class="flex items-center justify-between">
      <div class="pt-2">
        <img src="@/assets/img/logo.svg" alt="main_logo" />
      </div>
      <div class="hidden space-x-6 md:flex">
        <a
          href="#"
          class="hover:text-gray-400"
          v-for="(navItem, index) in navItems"
          :key="index"
          >{{ navItem }}</a
        >
      </div>
      <a
        class="hidden p-3 px-6 pt-2 text-white bg-red-500 hover:bg-red-600 hover:shadow-xl rounded-full self-baseline transition duration-150 ease-in-out md:block"
        href="#"
        >Get Started</a
      >
      <button
        :class="{ open: isOpen }"
        class="block hamburger md:hidden focus:outline-none"
        id="menu-btn"
        @click="toggleMenu"
      >
        <span class="hamburger-top"></span>
        <span class="hamburger-middle"></span>
        <span class="hamburger-bottom"></span>
      </button>
    </div>

    <div class="md:hidden">
      <div
        v-show="isOpen"
        class="absolute flex flex-col items-center self-end py-8 mt-10 space-y-6 font-bold bg-white sm:w-auto sm:self-center left-6 right-6 drop-shadow-md"
        id="menu"
      >
        <a href="#">Pricing</a>
        <a href="#">Product</a>
        <a href="#">About Us</a>
        <a href="#">Careers</a>
        <a href="#">Community</a>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
      navItems: ["Pricing", "Product", "About Us", "Careers", "Community"],
    };
  },
  methods: {
    toggleMenu() {
      this.isOpen = !this.isOpen;
    },
  },
};
</script>

<style>
.hamburger {
  position: relative;
  width: 24px;
  height: 24px;
  cursor: pointer;
  transition: all 0.25s;
}
.hamburger-top,
.hamburger-middle,
.hamburger-bottom {
  position: absolute;
  top: 0;
  left: 0;
  width: 24px;
  height: 2px;
  background: #000;
  transform: rotate(0);
  transition: all 0.5s;
}
.hamburger-middle {
  transform: translateY(7px);
}
.hamburger-bottom {
  transform: translateY(14px);
}
.open {
  transform: rotate(90deg);
  transform: translateY(0px);
}
.open .hamburger-top {
  transform: rotate(45deg) translateY(6px) translate(6px);
}
.open .hamburger-middle {
  display: none;
}
.open .hamburger-bottom {
  transform: rotate(-45deg) translateY(6px) translate(-6px);
}
</style>
