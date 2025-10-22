<template>
  <div class="main-container">
    <NavBar />
    <router-view />
    <Footer />
  </div>
</template>

<script setup>
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';
</script>

<style scoped>
.main-container {
  width: 100%;
  position: relative;
  padding-top: 80px;
}

@media (max-width: 1200px) {
  .main-container {
    padding-top: calc(70px + 55px);
  }
}

@media (max-width: 480px) {
  .main-container {
    padding-top: calc(60px + 50px);
  }
}
</style>
