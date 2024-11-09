<template>
  <section id="intro" class="b">
    <h1>Hi I'm Dylane Russel, frontend developer based in Canada.</h1>
    <p>
      I am a FrontEnd Developer and Awwwards Young Jury from Cameroon, I’m passionate about creating
      beautiful, intuitive and responsive websites
    </p>
    <ReseauxSociaux />
    <a class="button" href="">MORE ABOUT ME</a>
  </section>
</template>

<script lang="ts" setup>
import ReseauxSociaux from './ReseauxSociaux.vue'
</script>

<style lang="scss" scoped>
@use '../assets/styles/abstracts/mixins' as *;
@use '../assets/styles/abstracts/variables' as *;

#intro{
  @include flex-column;
  padding-top: 150px;
  gap: $spacing-lg;
}
</style>
