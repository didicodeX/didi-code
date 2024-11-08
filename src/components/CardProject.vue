<template>
    <div class="card">
      <div class="card__header">
        <img :src="props.img" alt="">
      </div>
      <div class="card__body">
        <h4 class="card__title">{{ props.categorie }}</h4>
        <a :href="props.link" class="card__link">Voir le projet</a>
      </div>
      <h4 class="card__subtitle">{{ props.name }}</h4>
    </div>
</template>

<script lang="ts" setup>
const props = defineProps<{
  categorie: string;
  name: string;
  link: string;
  img: string;
}>();
</script>

<style lang="scss" scoped>
.card {
  border-radius: 5px;
  width: 200px;
  background-color: white;
  color: #333;
  background-color: red;
}
.card__header {
  background-color: #f0f0f0;
  border-bottom: 1px solid #ccc;
}
.card__title {
  margin: 0;
}
.card__body {
  padding: 10px;
  display: flex;
  align-items: baseline;
  gap: 10px;
}
.card__subtitle {
  margin: 0;
}
.card__link {
  color: #007bff;
  display: block;
  margin-top: 10px;
  text-decoration: none;
}
.card__link:hover {
  text-decoration: underline;
}
</style>
