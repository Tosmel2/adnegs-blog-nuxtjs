<template>
  <header class="py-4 bg-white shadow">
    <nav class="md:w-[80%] w-[90%] flex items-center justify-between mx-auto">
      <!-- Brand Name -->
      <div class="text-3xl font-bold">
        <a href="#" class="text-gray-900">Adnegs.</a>
      </div>
      
      <!-- Hamburger Icon (only visible on mobile) -->
      <div class="md:hidden">
        <button @click="isOpen = !isOpen" class="text-gray-600 focus:outline-none">
          <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
          </svg>
        </button>
      </div>

      <!-- Navigation Links (hidden on mobile, shown on desktop) -->
      <ul :class="{'hidden': !isOpen}" class="hidden space-x-8 md:flex">
        <li><a href="#" class="text-gray-600 hover:text-black">Home</a></li>
        <li><a href="#" class="text-gray-600 hover:text-black">Categories</a></li>
        <li><a href="#" class="text-gray-600 hover:text-black">Feature</a></li>
        <li><a href="#" class="text-gray-600 hover:text-black">About</a></li>
      </ul>

      <!-- Social Icons (hidden on mobile, shown on desktop) -->
      <div :class="{'hidden': !isOpen}" class="hidden space-x-4 md:flex">
        <a href="#" class="text-gray-600 hover:text-black"><i class="fab fa-facebook"></i></a>
        <a href="#" class="text-gray-600 hover:text-black"><i class="fab fa-twitter"></i></a>
        <a href="#" class="text-gray-600 hover:text-black"><i class="fab fa-instagram"></i></a>
      </div>

      <!-- Mobile Menu (shown when isOpen is true) -->
      <div v-if="isOpen" class="absolute left-0 z-20 w-full py-5 bg-white shadow-lg top-16 md:hidden">
        <ul class="flex flex-col items-center gap-4 py-4 space-y-4">
          <li><a href="#" class="text-gray-600 hover:text-black">Home</a></li>
          <li><a href="#" class="text-gray-600 hover:text-black">Categories</a></li>
          <li><a href="#" class="text-gray-600 hover:text-black">Feature</a></li>
          <li><a href="#" class="text-gray-600 hover:text-black">About</a></li>
          <div class="flex space-x-4">
            <a href="#" class="text-gray-600 hover:text-black"><i class="fab fa-facebook"></i></a>
            <a href="#" class="text-gray-600 hover:text-black"><i class="fab fa-twitter"></i></a>
            <a href="#" class="text-gray-600 hover:text-black"><i class="fab fa-instagram"></i></a>
          </div>
        </ul>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      isOpen: false // State to control mobile menu visibility
    };
  }
}
</script>

<style scoped>
</style>

