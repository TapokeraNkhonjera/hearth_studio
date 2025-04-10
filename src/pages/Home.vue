<template>
  <div>
    <!-- Navbar Component -->
    <Navbar />

    <!-- Hero Section with Background Image -->
    <section class="text-center py-32 px-6 bg-cover bg-center bg-no-repeat">
      <HeroSection />
    </section>
  </div>
</template>

<script>
import HeroSection from '../components/HeroSection.vue'
import Navbar from '../components/NavBar.vue'

export default {
  components: {
    HeroSection,
    Navbar
  }
}
</script>

<style scoped>
/* Optional: additional styling for the home page */
</style>
