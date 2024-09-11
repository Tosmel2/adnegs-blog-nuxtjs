<script setup>
import hero_img from '@/assets/images/hero_img.webp';
import jason from '@/assets/images/jason.png';
</script>
<template>
  <main class="">
    <div class="mx-auto md:w-[80%] w-[90%] md:py-10 py-5">
      <div class="relative w-full rounded-md mb-[10rem]">
        <img :src="hero_img" alt="" class=" object-cover  w-full h-[400px]  sm:h-[600px]  rounded-lg">
        <div class=" shadow flex flex-col max-w-[300px] sm:max-w-[500px] gap-4 absolute bottom-[2rem] md:bottom-[-4rem] md:left-[5%] p-[20px]  rounded-lg md:bg-[#fff] 
            md:border md:border-[#E8E8EA] md:dark:bg-[#181A2A] md:dark:border-[#242535]">
            <p class=" text-sm bg-[#4B6BFB] shadow text-white w-max p-2 rounded">Technology</p>
            <p class=" text-[0.8rem] sm:text-4xl text-white md:text-black font-semibold dark:md:text-[#fff]">The
                Impact of
                Technology on the Workplace: How Technology is Changing
            </p>
        <div
            class="flex flex-col md:flex-row  md:items-center gap-5 text-white md:text-[#97989F] font-medium mt-2">
            <div class="flex items-center gap-3">
                <img :src="jason" alt="">
                <p>Jason Francisco</p>
            </div>
            <p>August 20, 2022</p>
          </div>
        </div>
      </div>
    </div>
  </main>

</template>