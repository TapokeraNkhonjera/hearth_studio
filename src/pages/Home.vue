<template>
  <div>
    <!-- Navbar Component -->
    <Navbar />

    <!-- Hero Section with Background Image -->
    <section class="text-center py-32 px-6 bg-cover bg-center bg-no-repeat">
      <HeroSection />
    </section>
<!-- Services Section -->
    <section>
      <ServicesSection />
    </section>
    
    <!-- Carousel Section -->
    <section>
      <CarouselSection />
    </section>

    
  </div>
</template>

<script>
import HeroSection from '../components/HeroSection.vue'
import Navbar from '../components/NavBar.vue'
import ServicesSection from '../components/ServicesSection.vue'
import CarouselSection from '../components/CarouselSection.vue'

export default {
  components: {
    HeroSection,
    Navbar,
    ServicesSection,
    CarouselSection
  }
}
</script>

<style scoped>
/* Add your custom styles here if needed */
</style>
