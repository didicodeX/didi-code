<!-- ParentComponent.vue -->
<script lang="ts" setup>
import { ref } from 'vue'
import EnfantComponent from './EnfantComponent.vue'

// Définition d'un message initial
const parentMessage = ref('Bonjour depuis le Parent')

// Fonction pour mettre à jour le message lorsque l’événement est reçu de l’enfant
function handleUpdate(newValue: string) {
  parentMessage.value = newValue
}
</script>

<template>
  <div>
    <h2>Composant Parent</h2>
    <p>Message actuel : {{ parentMessage }}</p>
    <a href="https://fonts.google.com/">google font</a>
    <img src="../assets/icons/sun.svg" alt="">
    <img src="../assets/icons/moon.svg" alt="">

    <!-- Transmission de la prop `message` et écoute de l'événement `update` -->
    <EnfantComponent :message="parentMessage" @update="handleUpdate" />
  </div>
</template>

<style lang="scss" scoped>
// @use '../assets/styles/style.scss' as *;
a {
  background-color: red;
}
</style>
