<template>
  <body class="bg-blue-500">
    <nav class="px-4 py-4 flex justify-between top-0 sticky z-50 bg-white">
      <div class="flex justify-between max-w-6xl mx-auto">

          <a class="text-3xl font-bold leading-none" href="#">
          <span class="font-bold text-3xl">CrynTek</span>
        </a>
        
        <ul class="hidden justify-between md:flex md:mx-auto md:space-x-6">
          <!-- md:w-auto  -->
          <li>
            <a class="text-sm text-gray-400 hover:text-gray-500" href="#">Home</a>
          </li>
          <li>
            <a class="text-sm text-blue-600 font-bold" href="#">Skills&Tools</a>
          </li>
  
          <li>
            <a class="text-sm text-gray-400 hover:text-gray-500" href="#"
              >Contact</a
            >
          </li>
        </ul>
      </div>
      <div class="md:hidden">
        <button class="navbar-burger flex items-center text-blue-600 p-3">
          <svg
            class="block h-4 w-4 fill-current"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"></path>
          </svg>
        </button>
      </div>
    </nav>
    <div class="navbar-menu relative z-50 hidden">
      <div class="navbar-backdrop fixed inset-0 bg-gray-800 opacity-25"></div>
      <nav
        class="
          fixed
          top-0
          left-0
          bottom-0
          flex flex-col
          w-5/6
          max-w-sm
          py-6
          px-6
          bg-white
          border-r
          overflow-y-auto
        "
      >
        <div class="flex items-center mb-8">
          <a class="mr-auto text-3xl font-bold leading-none" href="#">
            <span class="font-bold text-3xl">CrynTek</span>
          </a>
          <button class="navbar-close">
            <svg
              class="h-6 w-6 text-gray-400 cursor-pointer hover:text-gray-500"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M6 18L18 6M6 6l12 12"
              ></path>
            </svg>
          </button>
        </div>
        <div>
          <ul>
            <li class="mb-1">
              <a
                class="
                  block
                  p-4
                  text-sm
                  font-semibold
                  text-gray-400
                  hover:bg-blue-50 hover:text-blue-600
                  rounded
                "
                href="#"
                >Home</a
              >
            </li>
            <li class="mb-1">
              <a
                class="
                  block
                  p-4
                  text-sm
                  font-semibold
                  text-gray-400
                  hover:bg-blue-50 hover:text-blue-600
                  rounded
                "
                href="#"
                >Skills&Tools</a
              >
            </li>
            <li class="mb-1">
              <a
                class="
                  block
                  p-4
                  text-sm
                  font-semibold
                  text-gray-400
                  hover:bg-blue-50 hover:text-blue-600
                  rounded
                "
                href="#"
                >Contact</a
              >
            </li>
          </ul>
        </div>
        <div class="mt-auto">
          <p class="my-4 text-xs text-center text-gray-400">
            <span>Copyright ?? 2021</span>
          </p>
        </div>
      </nav>
    </div>
  </body>
</template>

<script>
// Burger menus
document.addEventListener("DOMContentLoaded", function () {
  // open
  const burger = document.querySelectorAll(".navbar-burger");
  const menu = document.querySelectorAll(".navbar-menu");

  if (burger.length && menu.length) {
    for (var i = 0; i < burger.length; i++) {
      burger[i].addEventListener("click", function () {
        for (var j = 0; j < menu.length; j++) {
          menu[j].classList.toggle("hidden");
        }
      });
    }
  }

  // close
  const close = document.querySelectorAll(".navbar-close");
  const backdrop = document.querySelectorAll(".navbar-backdrop");

  if (close.length) {
    for (var i = 0; i < close.length; i++) {
      close[i].addEventListener("click", function () {
        for (var j = 0; j < menu.length; j++) {
          menu[j].classList.toggle("hidden");
        }
      });
    }
  }

  if (backdrop.length) {
    for (var i = 0; i < backdrop.length; i++) {
      backdrop[i].addEventListener("click", function () {
        for (var j = 0; j < menu.length; j++) {
          menu[j].classList.toggle("hidden");
        }
      });
    }
  }
});
</script>

<style>
</style>