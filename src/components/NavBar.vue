<template>
  <nav class="navbar">
    <div class="navbar-container">
      <ul class="nav-links">
        <li><router-link to="/">HOME</router-link></li>
        <li><router-link to="/about">ABOUT</router-link></li>
        <li><router-link to="/portfolio">PORTFOLIO</router-link></li>
        <li><router-link to="/services">SERVICES</router-link></li>
        <li><router-link to="/blog">BLOG</router-link></li>
        <li><router-link to="/contact">CONTACT</router-link></li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navbar',
}
</script>

<style scoped>
.navbar {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background-color: rgba(255, 255, 255, 0); /* transparent */
  z-index: 1000;
  padding: 1rem 2rem;
}

.navbar-container {
  max-width: 1200px;
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 6rem;
  padding: 0;
  margin: 0;
}

.nav-links li a {
  color: #ffffff;
  text-decoration: none;
  font-size: 0.7rem;
  font-family: Montserrat;
  font-weight: 500;
  transition: color 0.3s ease;
}

.nav-links li a:hover {
  color: #cecece;
}
</style>
