<template>
    <section class="services-section">
      <h2 class="section-title">Our Core Services</h2>
      <div class="services-container">
        <div class="service-card">
          <div class="icon-wrapper">
            <img src="../assets/images/interior_design.png" alt="Interior Styling" class="icon-image" />
          </div>
          <div class="info">
            <h3>Interior Styling</h3>
            <p>Curating interiors that blend form and function with natural materials and timeless design principles.</p>
          </div>
        </div>
  
        <div class="service-card">
          <div class="icon-wrapper">
            <img src="../assets/images/visual_branding.png" alt="Visual Branding" class="icon-image" />
          </div>
          <div class="info">
            <h3>Visual Branding</h3>
            <p>Developing organic, authentic visual identities that reflect your story and connect with your audience.</p>
          </div>
        </div>
  
        <div class="service-card">
          <div class="icon-wrapper">
            <img src="../assets/images/spacial_planning.png" alt="Spatial Planning" class="icon-image" />
          </div>
          <div class="info">
            <h3>Spatial Planning</h3>
            <p>Designing thoughtful layouts that maximize flow, light, and harmony across residential and commercial spaces.</p>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: 'ServicesSection',
  }
  </script>
  
  <style scoped>
  .services-section {
    padding: 4rem 2rem;
    background-color: #f6f4f2;
    text-align: center;
    font-family: 'Montserrat', sans-serif;
  }
  
  .section-title {
    font-size: 2rem;
    margin-bottom: 2.5rem;
    color: #333;
    letter-spacing: 1px;
  }
  
  .services-container {
    display: flex;
    justify-content: center;
    gap: 2rem;
    flex-wrap: wrap;
  }
  
  .service-card {
    background-color: white;
    border-radius: 12px;
    padding: 2rem;
    width: 280px;
    overflow: hidden;
    transition: all 0.3s ease;
    position: relative;
  }
  
  .icon-wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 120px;
    margin-bottom: 0;
  }
  
  .icon-image {
    width: 64px;
    height: 64px;
    object-fit: contain;
    transition: transform 0.3s ease;
  }
  
  .info {
    opacity: 0;
    transform: translateY(-20px);
    transition: opacity 0.3s ease, transform 0.3s ease;
    margin-top: 1rem;
  }
  
  .service-card:hover .info {
    opacity: 1;
    transform: translateY(0);
  }
  
  .service-card h3 {
    font-size: 1.25rem;
    margin-bottom: 0.5rem;
    color: #2e2e2e;
  }
  
  .service-card p {
    font-size: 0.95rem;
    color: #555;
    line-height: 1.5;
  }
  </style>
  