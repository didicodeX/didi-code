<template>
  <div>
    <button class="button">button</button>
    <ReseauxSociaux />
    <skills-images />
  </div>
</template>
<script setup lang="ts">
import ReseauxSociaux from './components/ReseauxSociaux.vue'
import SkillsImages from './components/SkillsImages.vue'
</script>
<style lang="scss" scoped>
@use './assets/styles/components/index.scss' as *;
</style>
