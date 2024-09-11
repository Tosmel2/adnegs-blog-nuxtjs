<template>
  <section class="py-12 bg-gray-50">
    <div class="mx-auto w-[95%] md:w-[80%]">
      <h2 class="mb-6 text-xl font-bold text-gray-900 md:text-2xl">Latest Articles</h2>
    
      <!-- Article Grid -->
      <div class="grid grid-cols-1 gap-8 md:grid-cols-3">
        <div v-for="article in articles" :key="article?.title">
          <BlogCard :article="article" />
         
        </div>
        <!-- <div v-for="(article, index) in articles" :key="index" class="overflow-hidden bg-white rounded-lg shadow-lg">
          <img :src="article.image" alt="Article image" class="object-cover w-full h-48">
          <div class="p-4">
            <div class="flex items-center justify-between mb-2">
              <p class="text-sm text-gray-600">{{ article.author }}</p>
              <p class="text-xs text-gray-500">{{ article.category }}</p>
            </div>
            <h3 class="mb-2 text-lg font-semibold">{{ article.title }}</h3>
            <p class="text-sm text-gray-500">{{ article.description }}</p>
          </div>
          <div class="flex items-center justify-between p-4 text-gray-500 border-t">
            <div class="flex space-x-4">
              <span>{{ article.views }} Views</span>
              <span>{{ article.likes }} Likes</span>
              <span>{{ article.comments }} Comments</span>
            </div>
            <a href="#" class="text-red-500 hover:text-red-600">
              <i class="fas fa-arrow-right"></i>
            </a>
          </div>
        </div> -->
      </div>
    </div>
  </section>
</template>

<script setup>
const { data, status } = await useFetch("/api/articles")
  const articles = computed(() => {
      if (data.value?.status === 200) {
          return data.value?.data?.articles || [];
      }
  })
  // const { data: articles } = await useFetch('https://newsapi.org/v2/everything?q=tesla&from=2024-08-10&sortBy=publishedAt&apiKey=b85bd9dcd1a84160a66f5f4ad789555e')

// export default {
//   name: "BlogSection",
//   data() {
//     return {
//       articles: [
//         {
//           image: "https://via.placeholder.com/300",
//           author: "Steve Jobs",
//           title: "Content Marketing Strategies: Explore content trend",
//           description: "The Future of Artificial Intelligence: Trends and Implications.",
//           category: "Technologies",
//           views: "2,124",
//           likes: "735",
//           comments: "735"
//         },
//         {
//           image: "https://via.placeholder.com/300",
//           author: "Steve Jobs",
//           title: "Content Marketing Strategies: Explore content trend",
//           description: "The Future of Artificial Intelligence: Trends and Implications.",
//           category: "Technologies",
//           views: "2,124",
//           likes: "735",
//           comments: "735"
//         },
//         {
//           image: "https://via.placeholder.com/300",
//           author: "Steve Jobs",
//           title: "Content Marketing Strategies: Explore content trend",
//           description: "The Future of Artificial Intelligence: Trends and Implications.",
//           category: "Technologies",
//           views: "2,124",
//           likes: "735",
//           comments: "735"
//         },
//         {
//           image: "https://via.placeholder.com/300",
//           author: "Steve Jobs",
//           title: "Content Marketing Strategies: Explore content trend",
//           description: "The Future of Artificial Intelligence: Trends and Implications.",
//           category: "Technologies",
//           views: "2,124",
//           likes: "735",
//           comments: "735"
//         },
//         {
//           image: "https://via.placeholder.com/300",
//           author: "Steve Jobs",
//           title: "Social Media Marketing: Cover social media strategies",
//           description: "The Future of Artificial Intelligence: Trends and Implications.",
//           category: "Technologies",
//           views: "2,124",
//           likes: "735",
//           comments: "735"
//         },
//         {
//           image: "https://via.placeholder.com/300",
//           author: "Steve Jobs",
//           title: "Data Privacy and Ethics in the Digital Age",
//           description: "The Future of Artificial Intelligence: Trends and Implications.",
//           category: "Technologies",
//           views: "2,124",
//           likes: "735",
//           comments: "735"
//         },
//         // Add more articles as needed
//       ]
//     };
//   }
// };
</script>

<style scoped>
</style>
