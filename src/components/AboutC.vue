<template>
  <section id="about" class="b">
    <h2>About Me</h2>
    <div class="about__content">
      <p>
        Praesent malesuada mi nisi, quis tempus magna venenatis ut. Suspendisse tempor sem at
        scelerisque congue. Curabitur mollis, mi id molestie finibus, metus sem sagittis nunc,
        euismod feugiat orci neque non lorem. Aenean sollicitudin erat eu molestie tempus. Nunc ac
        eros elementum, fermentum lacus at, pellentesque mauris. Suspendisse eros neque, interdum
        euismod consectetur convallis, porttitor at massa. Phasellus a ultrices arcu. Donec viverra,
        lorem in pellentesque euismod, libero justo gravida nibh, non ultricies justo purus ultrices
        est. Ut at interdum dui. Donec ut ante ex. Maecenas id ex eget nibh consequat accumsan.
        Proin semper semper dui nec feugiat. Donec cursus neque id aliquet finibus. Morbi facilisis
        turpis nibh, nec dictum orci dictum nec. In hac habitasse platea dictumst. Maecenas mollis
        turpis vitae turpis bibendum, vitae tristique arcu eleifend.
      </p>
      <div class="me">
        <img src="../assets/img/moi.png" alt="" />
        <a class="button" href="">Download CV</a>
      </div>
      <article>
      <h2>Skills</h2>
      <skills-images />
    </article>
    </div>


  </section>
</template>

<script lang="ts" setup>
import SkillsImages from './SkillsImages.vue'
</script>

<style lang="scss" scoped>
@use '../assets/styles/abstracts/variables' as *;
@use '../assets/styles/abstracts/mixins' as *;
article {
  margin-top: $spacing-lg;
}
.about__content {
@include flex-center(space-between);
// flex-wrap: wrap;

p {
  width: 70%;
}
}
#about {
  @include flex-column;
}

.me {
  @include flex-column;
  gap: $spacing-lg;

  a{
    margin-left: auto;
  }
}

</style>
