<template>
  <div class="card">
    <div class="card__header">
      <img :src="props.img" alt="" />
    </div>
    <div class="card__body">
      <h4 class="card__categorie">{{ props.categorie }}</h4>
      <a class="card__link" :href="props.link" target="_blank">Voir le projet</a>
    </div>
    <h4 class="card__name">{{ props.name }}</h4>
  </div>
</template>

<script lang="ts" setup>
const props = defineProps<{
  categorie: string
  name: string
  link: string
  img: string
}>()
</script>

<style lang="scss" scoped>
@use '../assets/styles/abstracts/variables' as *;

.card {
  width: 250px;
  color: $primary-color;
  background-color: $text-color;


  &__header {
    height: 300px;
    overflow: hidden;
    img {
      object-fit: cover;
      width: 100%;
      height: 100%;
    }
  }
  &__body {
    padding: $spacing-xs;
    padding-left: $spacing-md;
    display: flex;
    align-items: baseline;
    gap: $spacing-xs;
  }
  &__categorie {
    color: $gray;
  }
  &__link {
    color: $primary-color;

    &:hover {
      text-decoration: underline;
    }
  }
  &__name {
    padding-left: $spacing-md;
    padding-bottom: $spacing-xs;
  }
}
</style>
