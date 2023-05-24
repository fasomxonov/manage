<template>
  <div class="bg-red-500 cta">
    <div
      class="container flex flex-col items-center justify-between px-6 py-24 mx-auto space-y-12 md:py-12 md:flex-row md:space-y-0"
    >
      <h2
        class="text-5xl font-bold leading-tight text-center text-white md:text-4xl md:max-w-xl md:text-left"
      >
        Simplify how your team works today
      </h2>
      <div>
        <a
          class="p-3 px-6 pt-2 text-red-500 hover:text-white shadow-2xl bg-white hover:bg-red-400 hover:ring-2 ring-white hover:shadow-xl rounded-full self-baseline transition duration-150 ease-in-out"
          href="#"
          >Get Started</a
        >
      </div>
    </div>
  </div>
</template>

<style>
.cta {
  background-image: url("@/assets/img/bg-simplify-section-desktop.svg");
  background-repeat: no-repeat;
}
@media(max-width: 576px) {
    .cta {
        background-image: url('@/assets/img/bg-simplify-section-mobile.svg');
    }
}
</style>
