<template>
  <section class="hero-section">
    <!-- Logo -->
    <div class="logo-container">
      <img :src="logoUrl" alt="Hearth Studios Logo" class="logo" />
    </div>

    <!-- Button -->
    <button class="start-button">
      START YOUR PROJECT
    </button>
  </section>
</template>

<script>
import backgroundImage from '../assets/images/background.png'
import logo from '../assets/images/primarylogo.png'

export default {
  name: 'HeroSection',
  data() {
    return {
      backgroundUrl: backgroundImage,
      logoUrl: logo,
    }
  }
}
</script>

<style scoped>
.hero-section {
  background-image: url('../assets/images/background.png');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  height: 100vh;
  width: 100vw;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 0;
  margin: 0;
  position: relative;
  text-align: center;
}

.logo {
  width: 26rem;
  height: auto;
  margin-bottom: 2rem;
  padding-bottom: 60px;
  padding-top: 40px;
}

.start-button {
  background-color: transparent;
  border: 0.5px solid white;
  color: white;
  padding: 6px 12px;
  font-size: 0.7rem;
  font-family: 'Montserrat', sans-serif;
  letter-spacing: 2px;
  border-radius: 6px;
  cursor: pointer;
  transition: all 0.8s ease;
}

.start-button:hover {
  background-color: white;
  color: black;
}
</style>

<style>
/* Global Reset (should go in App.vue or main.css, not inside scoped!) */
html, body {
  margin: 0;
  padding: 0;
  height: 100%;
  overflow-y: auto;
  scrollbar-width: none; /* Firefox */
}

body::-webkit-scrollbar {
  display: none; /* Chrome, Safari, Opera */
}
</style>
