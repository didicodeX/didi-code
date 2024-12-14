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
// import figmaCourseChatbot from '../assets/img/figmaCourseSite.png'
import Calculatrice from '../assets/img/calculatrice.png'
import figmaCourseSite from '../assets/img/figmaCourseSite.png'
import diane from '../assets/img/diane.png'
import CardProject from './CardProject.vue'
const projects = ref([
{
    id: 1,
    name: 'Figma Course',
    link: 'https://www.figma.com/design/qZBIuCbbhoCynV8NzHtxMc/Figma-Courses---Site?node-id=0-1&node-type=canvas&t=JVGCaL3sxRtG1a3x-0',
    img: figmaCourseSite,
    categorie: 'Design Figma',
  },
  {
    id: 2,
    name: 'Figma course',
    link: 'https://figma-courses.vercel.app/',
    img: figmaCourseSite,
    categorie: 'Integration',
  },
  {
    id: 3,
    name: 'Diane',
    link: 'https://diane-sale.vercel.app/',
    img: diane,
    categorie: 'Website',
  },
  {
    id: 4,
    name: 'Calculatrice',
    link: 'https://calculatrice-vanilla.vercel.app/',
    img: Calculatrice,
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
