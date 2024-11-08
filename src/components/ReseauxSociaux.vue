<template>
  <div>
    <img v-for="icon in icons" :key="icon.id" :src="icon.url" :alt="icon.name">
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const icons = ref([
  { id: 1, name: 'WhatsApp', url: '/src/assets/icons/bxl-whatsapp.svg' },
  { id: 2, name: 'GitHub', url: '/src/assets/icons/bxl-github.svg' },
  { id: 3, name: 'Email', url: '/src/assets/icons/bx-mail-send.svg' },
  { id: 4, name: 'LinkedIn', url: '/src/assets/icons/bxl-linkedin-square.svg' }
]);
</script>

<style lang="scss" scoped>
div {
  display: flex;
  gap: 26px;
}
</style>
