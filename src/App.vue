<template>
  <div class="app">
    <Navbar />
    <section id="intro" class="b1">

    </section>
    <section id="about" class="b2">

    </section>
    <section id="works" class="b3">

    </section>
    <section id="contact" class="b4">

    </section>
    <button class="button">button</button>
    <ReseauxSociaux />
    <skills-images />
    <CardsProjects/>
    <Footer/>
  </div>
</template>
<script setup lang="ts">
import Navbar from "./components/NavbarC.vue";
import ReseauxSociaux from './components/ReseauxSociaux.vue'
import SkillsImages from './components/SkillsImages.vue'
import CardsProjects from './components/CardsProjects.vue'
import Footer from './components/FooterC.vue'


</script>
<style lang="scss" scoped>
// @use './assets/styles/components/index.scss' as *;
@use './assets/styles/abstracts/variables' as *;

.app {
  padding: 0 $spacing-lg * 2;
}
section{
  height: 100vh;
}
</style>
