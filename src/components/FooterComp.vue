<template>
  <div class="bg-gray-900">
    <div
      class="container flex flex-col-reverse justify-between px-6 py-10 mx-auto space-y-8 md:flex-row md:space-y-0"
    >
      <div
        class="flex flex-col-reverse items-center justify-between space-y-12 md:flex-col md:space-y-0 md:items-start"
      >
        <div class="mx-auto my-6 text-center text-white md:hidden">Copyright &copy; 2023, All Rights Reserved</div>
        <div>
          <img
            class="h-8"
            src="@/assets/img/logo-white.svg"
            alt="footer-logo"
          />
        </div>
        <div class="flex justify-center space-x-4">
          <a href="#">
            <img
              class="h-8"
              src="../assets/img/icon-facebook.svg"
              alt="facebook-icon"
            />
          </a>
          <a href="#">
            <img
              class="h-8"
              src="../assets/img/icon-youtube.svg"
              alt="youtube-icon"
            />
          </a>
          <a href="#">
            <img
              class="h-8"
              src="../assets/img/icon-twitter.svg"
              alt="twitter-icon"
            />
          </a>
          <a href="#">
            <img
              class="h-8"
              src="../assets/img/icon-pinterest.svg"
              alt="pinterest-icon"
            />
          </a>
          <a href="#">
            <img
              class="h-8"
              src="../assets/img/icon-instagram.svg"
              alt="instagram-icon"
            />
          </a>
        </div>
      </div>

      <div class="flex justify-around space-x-32">
        <div class="flex flex-col space-y-3 text-white">
          <a class="hover:text-red-500" href="#">Home</a>
          <a class="hover:text-red-500" href="#">Pricing</a>
          <a class="hover:text-red-500" href="#">Products</a>
          <a class="hover:text-red-500" href="#">About</a>
        </div>
        <div class="flex flex-col space-y-3 text-white">
          <a class="hover:text-red-500" href="#">Careers</a>
          <a class="hover:text-red-500" href="#">Community</a>
          <a class="hover:text-red-500" href="#">Privacy Policy</a>
        </div>
      </div>

      <div class="flex flex-col justify-between">
        <form>
          <div class="flex space-x-3">
            <input
              class="flex-1 px-4 rounded-full focus:outline-none"
              type="text"
            />
            <button
              class="px-6 py-2 text-white rounded-full bg-red-500 hover:bg-red-400 focus:outline-none"
            >
              Go
            </button>
          </div>
        </form>
        <div class="hidden text-white md:block">
            Copyright &copy; 2023, All Rights Reserved
        </div>
      </div>
    </div>
  </div>
</template>
