<template>
  <div>
    <HeroSection />
    <AboutSection />
  </div>
</template>

<script>
import HeroSection from './components/HeroSection.vue'
import AboutSection from './components/AboutSection.vue'

export default {
  name: 'App',
  components: {
    HeroSection,
    AboutSection
  }
}
</script>

<style>
/* Global styles */
</style>
