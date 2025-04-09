<template>
  <section class="bg-green-200 text-center py-20 px-6">
    <h1 class="text-4xl font-bold text-gray-900 mb-4">Welcome to Hearth Studios</h1>
    <p class="text-lg text-gray-700 mb-8">
      Creating thoughtful, modern spaces with an earthy aesthetic.
    </p>
    <router-link to="/about">
      <button class="bg-green-500 text-white px-6 py-2 rounded-lg hover:bg-green-600 transition duration-300">
        Start Your Project
      </button>
    </router-link>
  </section>
</template>

<script>
export default {
  name: 'HeroSection'
}
</script>

<style scoped>
/* You can add any additional styles here */
</style>
