<template>
  <header class="nav">
    <div class="nav__links">
      <a class="nav__link" href="#intro">Accueil</a>
      <a class="nav__link" href="#about">À propos</a>
      <a class="nav__link" href="#works">Projets</a>
      <a class="nav__link" href="#contact">Contact</a>
    </div>
  </header>
</template>

<script lang="ts" setup></script>

<style lang="scss" scoped>
@use '../assets/styles/abstracts/variables' as *;
@use '../assets/styles/abstracts/mixins' as *;

@use 'sass:color';

.nav {
  @include flex-center(center);
  min-height: 50px;
  background-color: $secondary-color-transparent;
  position: fixed;
  left: 0;
  right: 0;
  z-index: 10;
  backdrop-filter: blur(10px);

  &__links {
    @include flex-center(center);
    gap: $spacing-xs;
    border-radius: 999px;
    width: max-content;
    padding: 10px $spacing-lg;
  }
  &__link {
    font-family: $font-title;
  }
}
</style>
