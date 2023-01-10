<template>
  <!-- <router-link to="/">LOGO</router-link> |
    <router-link to="/">Home</router-link> |
    <router-link to="/about">Information</router-link> |
    <router-link to="/about">Workshop</router-link>
    <h1>kfjojeg</h1>
    <router-view /> -->
  <nav class="bg-gray-100 top-0 sticky inset-x-0 mb-0 z-50">
    <div class="max-w-6xl mx-auto px-4">
      <div class="flex justify-between">
        <div class="flex space-x-4">
          <!-- logo -->
          <div>
            <a
              href="#"
              class="
                flex
                items-center
                py-5
                px-2
                text-gray-700
                hover:text-gray-900
              "
            >
              <i class="bx bxl-medium-old mr-1 text-xl mb-1 text-blue-400"></i>
              <span class="font-bold">CrynTek</span>
            </a>
          </div>
        </div>
        <!-- secondary nav -->
        <div class="hidden md:flex items-center space-x-1">
          <a href="/" class="py-5 px-3 ">Home</a>
          <a href="#info" class="py-5 px-3 ">Skills&Tools</a>
          <a href="#workshop" class="py-5 px-3 ">Workshop</a>
        </div>

      </div>
    </div>
  </nav>
  <!-- <div class="py-3 bg-red-500 h-screen p-3"></div> -->
</template>

<script>
export default {};
</script>

<style></style>
