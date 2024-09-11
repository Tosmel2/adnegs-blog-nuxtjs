<template>
  <div>
    <Header />
    <Hero />
    <Ads />
    <BlogSection />
    <Ads />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import BlogSection from './components/BlogSection.vue';
import Footer from './components/Footer.vue';
import Ads from './components/Ads.vue';

export default {
  components: {
    Header,
    Hero,
    BlogSection,
    Ads,
    Footer
  }
}
</script>

<style>
body {
  /* font-family: 'Inter', sans-serif; */
  font-family: 'Inter', Work Sans;
}
</style>
