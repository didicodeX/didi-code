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
    name: 'Figma course',
    link: 'https://figma-course-pi.vercel.app/',
    img: '/src/assets/img/figmaCourseChatbot.png',
    categorie: 'Integration',
  },
  {
    id: 2,
    name: 'Guide Kyoto',
    link: 'https://www.google.com',
    img: '/src/assets/img/KyotoSite.png',
    categorie: 'Website',
  },
  {
    id: 3,
    name: 'Figma Course',
    link: 'https://www.figma.com/design/qZBIuCbbhoCynV8NzHtxMc/Figma-Courses---Site?node-id=0-1&node-type=canvas&t=JVGCaL3sxRtG1a3x-0',
    img: '/src/assets/img/figmaCourseSite.png',
    categorie: 'Design Figma',
  },
  {
    id: 4,
    name: 'Diane',
    link: 'https://diane-sale.vercel.app/',
    img: '/src/assets/img/diane.png',
    categorie: 'Website',
  },
])
</script>

<style lang="scss" scoped>
@use '../assets/styles/abstracts//mixins' as *;
.cards {
  @include flex-center(center);
  width: 100%;
}
</style>
