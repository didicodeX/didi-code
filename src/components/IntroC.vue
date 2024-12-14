<template>
  <section id="intro">
    <h1>
      Salut, Je suis Dylane Tano, Mon objectif est clair :
      <span>devenir un développeur web accompli.</span>
    </h1>
    <img :src="moi" alt="" />

    <div class="flex">
      <div class="contact">
        <ReseauxSociaux />
        <a class="button" href="#about">PLUS SUR MOI</a>
      </div>
      <div class="me">
        <img :src="moi" alt="" />
        <a class="button" :href="cv" download="CV_Tano_Dylane.pdf"
          >Télécharger mon CV</a
        >
      </div>
    </div>
    <br /><br /><br />
  </section>
</template>

<script lang="ts" setup>
import ReseauxSociaux from './ReseauxSociaux.vue'
import moi from '../assets/img/moi.png'
import cv from '../assets/doc/CV_Tano_Dylane.pdf'
</script>

<style lang="scss" scoped>
@use '../assets/styles/abstracts/mixins' as *;
@use '../assets/styles/abstracts/variables' as *;
@use '../assets/styles/abstracts/utilities' as *;

#intro {
  @include flex-column;
  padding-top: 7rem;
  min-height: 100vh;

  @include xl {
    padding-top: 10rem;
    gap: 7rem;
  }

  @include xl {
    // padding-top: 10rem;
    // display: none;
  }

  gap: 2rem;

  & > img {
    border-radius: $radius;

    @include sm {
      display: none;
    }
    @include md {
      display: none;
    }
    @include lg {
      display: none;
    }
    @include xl {
      display: none;
    }
  }
}

.me {
  @include flex-column;
  gap: $spacing-md;
  margin-top: auto;
  img {
    border-radius: $radius;
    display: none;
    @include sm {
      display: block;
    }
    @include md {
      display: block;
    }
    @include lg {
      display: block;
    }
    @include xl {
      display: block;
    }
  }
  a {
    margin-left: auto;
    display: block;
  }
}
.contact {
  @include flex-column;
  margin-top: auto;
}

.flex {
  display: flex;
  // justify-content: space-between;
  width: 100%;
  @include sm {
    justify-content: center;
  }
}
h1 span {
  // text-decoration: underline;
  border-bottom: 4px solid $secondary-color;
  border-width: 10px;
}
// .flex {
// display: flex;
// // flex-wrap: wrap;
// }
</style>
