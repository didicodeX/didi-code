<template>
  <div class="cards">
    <CardProject
      v-for="{ id, name, link, img, categorie } in projects"
      :key="id"
      :categorie="categorie"
      :link="link"
      :name="name"
      :img="img"
    />
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue'
import CardProject from './CardProject.vue'
const projects = ref([
  {
    id: 1,
    name: 'Chatbot',
    link: 'https://www.amazon.com',
    img: '/src/assets/img/Chatbot.png',
    categorie: 'IA',
  },
  {
    id: 2,
    name: 'Resto Kyoto',
    link: 'https://www.google.com',
    img: '/src/assets/img/KyotoSite.png',
    categorie: 'Website',
  },
  {
    id: 3,
    name: 'Figma Course',
    link: 'https://www.googlefont.com',
    img: '/src/assets/img/figmaCourseSite.png',
    categorie: 'Figma',
  },
  {
    id: 4,
    name: 'Restaurant',
    link: 'https://lndev.me/',
    img: '/src/assets/img/restaurantSite.png',
    categorie: 'Website',
  },
])
</script>

<style lang="scss" scoped>
@use '../assets/styles/abstracts//mixins' as *;
.cards {
  @include flex-center(center);
}
</style>
