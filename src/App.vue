<template>
  <div id="app" class="font-sans text-gray-800">
    <HeroSection />
    <ResumeSection />
    <ContactSection />
  </div>
</template>

<script setup>
import HeroSection from './components/HeroSection.vue'
import ResumeSection from './components/ResumeSection.vue'
import ContactSection from './components/ContactSection.vue'
</script>

<style>
body {
  margin: 0;
  padding: 0;
  background-color:rgb(0, 0, 0), 254, 254, 0);
  scroll-behavior: smooth;
}

#app {
  max-width: 960px;
  margin: 0 auto;
  padding: 0 16px;
}
</style>
