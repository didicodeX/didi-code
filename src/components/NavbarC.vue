<template>
  <header class="nav">
    <a href="#" class="nav__logo">
      <img src="../assets/icons/me.svg" alt="logo" />
    </a>
    <div class="nav__links">
      <a class="nav__link" href="#intro">Intro</a>
      <a class="nav__link" href="#about">About</a>
      <a class="nav__link" href="#works">Works</a>
      <a class="nav__link" href="#contact">Contact</a>
    </div>
    <button class="nav__theme button">
      <i class="fa-regular fa-moon"></i>
    </button>
  </header>
</template>
<script lang="ts" setup></script>

<style lang="scss" scoped>
@use '../assets/styles/abstracts/variables' as *;
@use '../assets/styles/abstracts/mixins' as *;

.nav {
  @include flex-center(space-between);
  padding: $spacing-lg $spacing-xs;

  &__logo {
    border-radius: 100%;
    width: 35px;

    @include flex-center(center);
  }
  &__theme {
    background-color: $secondary-color;
    width: 40px;
    display: flex;
    justify-content: center;
    padding: $spacing-xs;
    border-radius: 100%;

    @include transition(background-color);
    &:hover {
      background-color: darken($secondary-color, 10%);
    }
  }
  &__logo {
    background-color: $text-color;
  }
  &__links {
    @include flex-center(center);
    gap: $spacing-xs;
    background-color: $secondary-color;
    padding: 15px;
    border-radius: 999px;
    width: 447px;
  }
  &__link {
    font-family: $font-title;
  }
}
</style>
