<!-- EnfantComponent.vue -->
<script lang="ts" setup>
import { defineProps, defineEmits } from 'vue';

// Définition de la prop `message` que le composant parent envoie
const props = defineProps<{
  message: string;
}>();

// Définition de l'événement `update` pour notifier le parent
const emit = defineEmits<{
  (event: 'update', newValue: string): void;
}>();

// Fonction pour émettre un événement `update` avec une nouvelle valeur
function notifyParent() {
  emit('update', 'Message mis à jour par l\'enfant');
}
</script>

<template>
  <div>
    <h2>Composant enfant</h2>
    <p>Message du parent : {{ props.message }}</p>
    <button @click="notifyParent">Mettre à jour le parent</button>
  </div>
</template>
