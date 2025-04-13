<template>
    <section class="carousel-section">
      <div class="carousel-wrapper">
        <div
          class="carousel-track"
          :style="{ transform: `translateX(-${currentIndex * 100}%)` }"
        >
          <div class="carousel-slide">
            <img src="../assets/images/carousel1.jpg" alt="Image 1" class="carousel-image" />
            <div class="carousel-text">
              <h2>Innovative Design</h2>
              <p>We craft spaces that transcend trends — spaces rooted in intention and
              driven by curiosity. Every project begins with a conversation and evolves
              into a tailored experience, where form, function, and emotion harmoniously
              collide. It's not just about aesthetics — it's about evoking a sense of
              place that endures.</p>
            </div>
          </div>
          <div class="carousel-slide">
            <img src="../assets/images/carousel2.jpg" alt="Image 2" class="carousel-image" />
            <div class="carousel-text">
              <h2>Modern Aesthetics</h2>
              <p>Our approach to modern design is quiet, deliberate, and deeply rooted in
              simplicity. We focus on clean lines, natural light, and considered
              materiality — all working in rhythm to create environments that feel both
              elevated and grounded. The result is timeless architecture that breathes,
              adapts, and invites.</p>
            </div>
          </div>
          <div class="carousel-slide">
            <img src="../assets/images/carousel3.jpg" alt="Image 3" class="carousel-image" />
            <div class="carousel-text">
              <h2>Thoughtful Solutions</h2>
              <p>Behind every beautiful space lies a series of intentional decisions. We
              embrace constraints as a canvas for creativity — offering bespoke solutions
              that balance innovation with practicality. Whether you're building from
              scratch or refining a vision, our work is shaped by insight, strategy, and
              care at every step.</p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: 'CarouselSection',
    data() {
      return {
        currentIndex: 0
      }
    },
    mounted() {
      this.startAutoSlide()
    },
    methods: {
      startAutoSlide() {
        setInterval(() => {
          this.currentIndex = (this.currentIndex + 1) % 3
        }, 6000)
      }
    }
  }
  </script>
  
  <style scoped>
  .carousel-section {
    width: 100vw;
    height: 100vh;
    margin: 0;
    padding: 0;
    overflow: hidden;
  }
  
  .carousel-wrapper {
    width: 100%;
    height: 100%;
    overflow: hidden;
    position: relative;
  }
  
  .carousel-track {
    display: flex;
    height: 100%;
    transition: transform 2s ease-in-out;
  }
  
  .carousel-slide {
    min-width: 100%;
    height: 100%;
    position: relative;
    box-sizing: border-box;
  }
  
  .carousel-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
  }
  
  .carousel-text {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
    font-family: Montserrat;
    color: white;
    background-color: rgba(0, 0, 0, 0.5);
    padding: 2rem;
    border-radius: 8px;
    max-width: 80%;
  }
  
  .carousel-text h2 {
    font-size: 1.5rem;
    margin-bottom: 1rem;
  }
  
  .carousel-text p {
    font-size: 0.8rem;
  }
  </style>
  