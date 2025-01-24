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
import ITSC from '../assets/img/ITSC.png'
import figmaCourseSite from '../assets/img/figmaCourseSite.png'
import api from "../assets/img/api.png"
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
    name: 'ITSC',
    link: 'https://www.figma.com/design/tztzfjlF7XtxDXpS5OGXGZ/ITSC?node-id=0-1&p=f&t=pAHqIRGF573gfzAS-0',
    img: ITSC,
    categorie: 'Design Figma',
  },
  {
    id: 4,
    name: 'myaddressesbook',
    link: 'https://api.myaddressesbook.com/docs/',
    img: api,
    categorie: 'API',
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
