<template>
  <div>
    <button class="button">button</button>
    <ReseauxSociaux />
    <skills-images />
    <CardsProjects/>
  </div>
</template>
<script setup lang="ts">
import ReseauxSociaux from './components/ReseauxSociaux.vue'
import SkillsImages from './components/SkillsImages.vue'
import CardsProjects from './components/CardsProjects.vue'



</script>
<style lang="scss" scoped>
@use './assets/styles/components/index.scss' as *;
</style>
