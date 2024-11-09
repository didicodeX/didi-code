<template>
  <section id="works" class="b">
    <h2>Works</h2>
    <p class="mini-title">Here are some of my favorite projects I have done lately. Feel free to check them out.</p>
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
  padding-top: $spacing-sm;
  gap: $spacing-lg;
}
</style>
