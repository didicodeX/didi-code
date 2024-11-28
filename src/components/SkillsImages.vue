<template>
  <div class="skills">
    <div v-for="{ id, name, url } in images" :key="id" class="skill">
      <img :src="url" :alt="name" />
      <p>{{ name }}</p>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import figma from '../assets/img/figma.png'
import html5 from '../assets/img/html5.png'
import scss from '../assets/img/scss.png'
import tailwindcss from '../assets/img/tailwindcss.png'
import typescript from '../assets/img/typescript.png'
import vuejs from '../assets/img/vuejs.png'
import seo from '../assets/img/seo.png'
import git from '../assets/img/git.png'

const images = ref([
  { id: 1, name: 'Figma', url: figma },
  { id: 2, name: 'HTML5', url: html5 },
  { id: 3, name: 'SCSS', url: scss },
  { id: 4, name: 'Tailwind', url: tailwindcss },
  { id: 5, name: 'TypeScript', url: typescript },
  { id: 6, name: 'Vue', url: vuejs },
  { id: 7, name: 'SEO', url: seo },
  { id: 8, name: 'Git', url: git },
])
</script>

<style lang="scss" scoped>
@use '../assets/styles/abstracts/mixins' as *;

.skills {
  @include flex-center;
}

.skill {
  @include flex-column(center, center);
  gap: 10px;
}

img {
  height: 30px;
  @include sm {
    height: 40px;
  }
  @include md {
    height: 50px;
  }
  @include lg {
    height: 60px;
  }
  @include xl {
    height: 70px;
  }
}
p {
  text-align: center;
}
</style>
