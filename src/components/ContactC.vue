<template>
  <section id="contact" class="b">
    <h2>Contact</h2>
    <p class="mini-title">
      I love to hear from you. Whether you have a question or just want to chat about design, tech &
      art shoot me a message.
    </p>
    <ReseauxSociaux />
    <a href="" class="button">SAY HELLO</a>
  </section>
</template>

<script lang="ts" setup>
import ReseauxSociaux from './ReseauxSociaux.vue'
</script>

<style lang="scss" scoped>
@use '../assets/styles/abstracts/mixins' as *;
#contact {
  @include flex-column;
  padding-top: 150px;
  // gap: $spacing-lg;
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
