<template>
  <div class="min-h-full p-4 overflow-hidden bg-white rounded-lg shadow">
    <img :src="article?.urlToImage || placeholder_img" alt="Article image" class="object-cover w-full h-48 rounded-md">
    <div class="p-2">
      <div class="flex items-center justify-between mb-2">
        <p class="text-md font-medium text-[#4B6BFB] bg-gray-100 rounded-md p-2">Technology</p>
        <p class="text-xs text-gray-500">{{ article?.category }}</p>
      </div>
      <h3 class="mb-2 text-lg font-semibold">{{ (article?.title || '').split(' ').slice(0, 12).join(' ') }}</h3>
      <p class="text-sm text-gray-500">{{ (article?.description || '').split(' ').slice(0, 20).join(' ') + '....' }}</p>
      <div
            class="flex flex-col md:flex-row  md:items-center md:justify-between text-white md:text-[#97989F] mt-3">
            <div class="flex items-center gap-2">
                <img :src="jason" alt="">
                <p class="text-sm">{{ (article?.author || 'Jason').split(' ').slice(0, 1).join(' ') }} </p>
            </div>
            <p class="text-sm">Aug 20, 2022</p>
          </div>
    </div>
  </div>
</template>

<script setup>
    import placeholder_img from '@/assets/images/placeholder_img.png';
    import jason from '@/assets/images/jason.png';
    const { article } = defineProps(['article'])
</script>

<style scoped>

</style>