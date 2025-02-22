<script setup lang="ts">
import { onMounted } from 'vue'
import AOS from 'aos'
import 'aos/dist/aos.css'
import HeroSection from './components/HeroSection.vue'

// Initialize AOS
onMounted(() => {
  AOS.init({
    duration: 1000,    // Duration of animation
    once: true,        // Whether animation should happen only once
    easing: 'ease-in-out',
    offset: 120,       // Offset (in px) from the original trigger point
    delay: 0,          // Default delay
  })
})
</script>

<template>
  <main>
    <!-- Hero section with fade-up animation -->
    <div data-aos="fade-up">
      <HeroSection />
    </div>

    <!-- Extra section with slide-right animation and delay -->
    <div 
      data-aos="fade-right"
      data-aos-delay="200"
      data-aos-duration="1200"
    >
      <extra />
    </div>

    <!-- Contact section with zoom-in animation -->
    <div 
      data-aos="zoom-in"
      data-aos-offset="300"
      data-aos-easing="ease-in-sine"
    >
      <contact />
    </div>

    <!-- Big page section with fade-up animation and longer duration -->
    <div 
      data-aos="fade-up"
      data-aos-duration="1500"
      data-aos-anchor-placement="top-center"
    >
      <BigPage />
    </div>
  </main>
</template>

<style>
/* Optional: Add some spacing between sections */
main > div {
  margin: 2rem 0;
}
</style>
