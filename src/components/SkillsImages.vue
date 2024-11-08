<template>
  <div class="skills">
    <div v-for="{ id, name, url } in images" :key="id">
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
  { id: 4, name: 'Bootstrap', url: '/src/assets/img/bootstrap.png' },
  { id: 5, name: 'Wordpress', url: '/src/assets/img/wordpress.png' },
  { id: 6, name: 'Javascript', url: '/src/assets/img/javascript.png' },
  { id: 7, name: 'SEO', url: '/src/assets/img/seo.png' },
  { id: 8, name: 'Git', url: '/src/assets/img/git.png' },
])
</script>

<style lang="scss" scoped>
@use '../assets/styles/abstracts/mixins' as *;

.skills {
    @include flex-center;
}
img {
  height: 61px;
}
p {
  text-align: center;
}
</style>
