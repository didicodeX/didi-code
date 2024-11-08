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
    <img src="/src/assets/img/figmaCourseSite.png" alt="">
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
    categorie: 'Figma design',
  },
  {
    id: 4,
    name: 'Portfolio',
    link: 'https://lndev.me/',
    img: '/src/assets/img/portfolio.png',
    categorie: 'Website',
  },
])
</script>

<style lang="scss" scoped>
.cards {
  display: flex;
  gap: 20px;
  justify-content: center;
}
</style>
