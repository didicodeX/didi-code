<template>
  <div>
    <a target="_blank" :href="link" v-for="{id, name, url, link} in icons" :key="id"><img :src="url" :alt="name"></a>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const icons = ref([
  { id: 1, name: 'WhatsApp', url: '/src/assets/icons/bxl-whatsapp.svg', link: "https://wa.me/15062331887"},
  { id: 2, name: 'GitHub', url: '/src/assets/icons/bxl-github.svg', link: "https://github.com/RusselTano" },
  { id: 3, name: 'Email', url: '/src/assets/icons/bx-mail-send.svg', link: "mailto:edtanola01@monccnb.ca"},
]);
</script>

<style lang="scss" scoped>
div {
  display: flex;
  gap: 24px;
}
a:nth-child(1):hover{
  filter: drop-shadow(0 0 0.75rem #25D366);
}
a:nth-child(2):hover{
  filter: drop-shadow(0 0 0.75rem #f1f1f1);
}
a:nth-child(3):hover{
  filter: drop-shadow(0 0 0.75rem #D93025);
}
</style>
