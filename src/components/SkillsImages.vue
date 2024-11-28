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

const images = ref([
  { id: 1, name: 'Figma', url: '/src/assets/img/figma.png' },
  { id: 2, name: 'HTML5', url: '/src/assets/img/html5.png' },
  { id: 3, name: 'SCSS', url: '/src/assets/img/scss.png' },
  { id: 4, name: 'Tailwind', url: '/src/assets/img/tailwindcss.png' },
  { id: 5, name: 'TypeScript', url: '/src/assets/img/typescript.png' },
  { id: 6, name: 'Vue', url: '/src/assets/img/vuejs.png' },
  { id: 7, name: 'SEO', url: '/src/assets/img/seo.png' },
  { id: 8, name: 'Git', url: '/src/assets/img/git.png' },
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
