<template>
  <section id="contact">
    <h2>Contact</h2>
    <h1>
      J'adore avoir de vos nouvelles. Que vous ayez une question ou que vous souhaitiez simplement discuter de design, de technologie et d'art, envoyez-moi un message.
    </h1>
    <ReseauxSociaux />
    <form action="mailto:edtanola01@monccnb.ca">
      <button class="button">DIRE BONJOUR</button>
    </form>
    <br>
  </section>
</template>


<script lang="ts" setup>
import ReseauxSociaux from './ReseauxSociaux.vue'
</script>

<style lang="scss" scoped>
@use '../assets/styles/abstracts/mixins' as *;
@use '../assets/styles/abstracts/variables' as *;
#contact {
  @include flex-column;
  gap: $spacing-xl;
  padding-top: 3.8rem;
  min-height: 80vh;
}
</style>

<!--
      <form action="">
        <input type="text" placeholder="Name" />
        <input type="email" placeholder="Email" />
        <textarea placeholder="Message"></textarea>
        <button class="button">Send</button>
      </form>

      Want to get in touch? I'd love to hear from you. Here's how you can reach me...
 -->
