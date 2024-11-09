<template>
  <div class="app">
    <Navbar />
    <Intro />
    <About />
    <Works />
    <Contact />
    <Footer />
  </div>
</template>
<script setup lang="ts">
import Navbar from './components/NavbarC.vue'
import Footer from './components/FooterC.vue'
import Intro from './components/IntroC.vue'
import About from './components/AboutC.vue'
import Works from './components/WorksC.vue'
import Contact from './components/ContactC.vue'
</script>

<style lang="scss" scoped>
@use './assets/styles/abstracts/variables' as *;

.app {
  padding: 0 $spacing-lg * 3.4;
}
</style>
