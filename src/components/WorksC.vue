<template>
  <section id="works">
    <h2>Projets</h2>
    <h1>Voici quelques-uns de mes projets préférés que j'ai réalisés récemment. N'hésitez pas à les découvrir.</h1>
    <CardsProjects />
  </section>
</template>

<script lang="ts" setup>
import CardsProjects from './CardsProjects.vue'
</script>

<style lang="scss" scoped>
@use '../assets/styles/abstracts/variables' as *;
@use '../assets/styles/abstracts/mixins' as *;
#works {
  @include flex-column;
  padding-top: 3.8rem;
  gap: $spacing-lg;
}
</style>
