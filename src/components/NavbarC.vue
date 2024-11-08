<template>
  <div class="nav">
    <div class="nav__logo">
      <a href="#">
        <img src="../assets/icons/me.svg" alt="logo" />
      </a>
    </div>
    <div class="nav__links">
      <a class="nav__link" href="#intro">Intro</a>
      <a class="nav__link" href="#about">About</a>
      <a class="nav__link" href="#works">Works</a>
      <a class="nav__link" href="#contact">Contact</a>
    </div>
    <div class="nav__theme">
      <a href="#">
        <i class="fa-regular fa-moon"></i>
      </a>
    </div>
  </div>
</template>
<script lang="ts" setup></script>

<style lang="scss" scoped>
@use '../assets/styles/abstracts/variables' as *;
@use '../assets/styles/abstracts/mixins' as *;

.nav {
  @include flex-center(space-between);
  padding: $spacing-xs;

  &__logo {
    border-radius: 100%;
    width: 35px;

    @include flex-center(center);
  }
  &__theme {
    background-color: $secondary-color;
    width: 35px;
    height: 35px;
    display: flex;
    justify-content: center;
    padding: 8px;
    border-radius: 100%;
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
