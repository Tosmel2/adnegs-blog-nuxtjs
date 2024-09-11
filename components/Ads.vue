<template>
  <div class="p-5 overflow-hidden bg-[#E8E8EA]">
    <div class="scroll-container">
      <div class="scroll-content">
        <div class="flex whitespace-nowrap">
          <span class="text-xl md:text-3xl font-bold text-[#4B6BFB] mr-5">Technology.</span>
          <span class="text-lg md:text-3xl font-bold text-[#f4d844] mr-5">Business.</span>
          <span class="text-lg md:text-3xl font-bold text-[#7ca736] mr-5">Sports.</span>
          <span class="text-lg mr-2 md:text-3xl font-bold text-[#8aaea7]">Travels.</span>
          
          <span class="text-lg md:text-3xl font-bold text-[#4B6BFB] mr-5 ml-2">Technology.</span>
          <span class="text-lg md:text-3xl font-bold text-[#f4d844] mr-5">Business.</span>
          <span class="text-lg md:text-3xl font-bold text-[#7ca736] mr-5">Sports.</span>
          <span class="text-lg mr-2 md:text-3xl font-bold text-[#8aaea7]">Travels.</span>
        </div>

        <!-- Duplicate content for smooth scroll -->
        <div class="flex whitespace-nowrap">
          <span class="text-xl md:text-3xl font-bold text-[#4B6BFB] mr-5">Technology.</span>
          <span class="text-lg md:text-3xl font-bold text-[#f4d844] mr-5">Business.</span>
          <span class="text-lg md:text-3xl font-bold text-[#7ca736] mr-5">Sports.</span>
          <span class="text-lg mr-2 md:text-3xl font-bold text-[#8aaea7]">Travels.</span>
          
          <span class="text-lg md:text-3xl font-bold text-[#4B6BFB] mr-5 ml-2">Technology.</span>
          <span class="text-lg md:text-3xl font-bold text-[#f4d844] mr-5">Business.</span>
          <span class="text-lg md:text-3xl font-bold text-[#7ca736] mr-5">Sports.</span>
          <span class="text-lg mr-2 md:text-3xl font-bold text-[#8aaea7]">Travels.</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
</script>

<style scoped>
.scroll-container {
  overflow: hidden; /* Hide overflow to prevent scrolling manually */
}

.scroll-content {
  display: flex;
  animation: scroll-horizontal 15s linear infinite;
}

@keyframes scroll-horizontal {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(-50%);
  }
}
</style>
