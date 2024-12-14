<template>
  <hr />
  <footer>
    <p>&copy; 2024 Dylane Tano. All rights reserved</p>
    <div class="to-Top">
      <a href="#" class="button">
        <svg
          width="11"
          height="10"
          viewBox="0 0 11 10"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M0.547102 9.04609H10.3893C10.4889 9.04578 10.5866 9.01829 10.6718 8.9666C10.757 8.9149 10.8265 8.84095 10.8728 8.75271C10.9191 8.66446 10.9404 8.56526 10.9345 8.46579C10.9286 8.36632 10.8957 8.27034 10.8393 8.18818L5.91821 1.07993C5.71425 0.785207 5.22324 0.785207 5.01874 1.07993L0.0976421 8.18818C0.0406803 8.27016 0.0072766 8.36619 0.00106018 8.46583C-0.00515624 8.56547 0.0160524 8.66491 0.0623818 8.75334C0.108711 8.84177 0.17839 8.91582 0.263846 8.96743C0.349303 9.01904 0.44727 9.04625 0.547102 9.04609ZM5.4682 2.35176L9.34602 7.95251H1.59037L5.4682 2.35176Z"
            fill="white"
          />
        </svg>
      </a>
    </div>
  </footer>
</template>

<script lang="ts" setup></script>

<style lang="scss" scoped>
@use '../assets/styles/abstracts/variables' as *;
@use '../assets/styles/abstracts/mixins' as *;

footer {
  @include flex-center(space-between);
  padding: $spacing-md 0;

  .to-Top {
    // @include flex-center(center);
    // border-radius: 100%;
    cursor: pointer;
    margin-left: auto;

    .button{
      // background-color: $primary-color;
      padding: $spacing-xs  $spacing-sm;
      border-radius: 100%;
    }
  }

}
</style>
