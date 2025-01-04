<template>
  <section id="about">
    <h2>A propos de moi</h2>
    <p>
      Je m'appelle Dylane Tano, j'ai 19 ans et je suis passionné par le développement web. Mon
      objectif est clair : devenir un développeur web accompli, spécialisé dans la création
      d'expériences utilisateur captivantes et fonctionnelles. Mon parcours a débuté en février
      2023, lorsque j'ai entrepris d'apprendre de manière autodidacte les bases du développement
      web. Actuellement, je poursuis mes études au Collège Communautaire du Nouveau-Brunswick
      (CCNB), au Canada, où je continue à affiner mes compétences et à élargir mes connaissances.
    </p>
    <h2>Mon Univers</h2>
    <p>
      J'ai toujours été fasciné par l'art et la beauté visuelle, une passion qui m'a amené à dessiner dès mon plus jeune âge. Aujourd'hui, cet amour de l'esthétique se reflète dans mon approche du développement front-end, où je cherche à allier design et fonctionnalité pour offrir des interfaces utilisateur attrayantes. J'aime également relever des défis et apprendre de nouvelles technologies, ce qui me pousse à me dépasser et à m'améliorer constamment.
    </p>
    <h2>Apprentissage et Exploration</h2>
    <p>Curieux et avide de savoir, j'ai exploré diverses plateformes pour me former :</p>
    <ul>
      <li><strong>YouTube</strong> : mon premier point de départ, où j'ai découvert les bases du code et de nombreuses ressources pédagogiques.</li>
      <li><strong>Udemy</strong> : j'y ai suivi des formations complètes proposées par des créateurs de contenu que j'admire.</li>
      <li><strong>Alphorm et Dyma</strong> : des plateformes spécialisées dans les technologies web, qui m'ont permis d'approfondir mes connaissances.</li>
      <li><strong>Formations indépendantes</strong> : proposées par des experts sur leurs propres sites.</li>
    </ul>
    <p>Chaque étape de mon apprentissage a renforcé ma soif de connaissance et ma volonté de continuer à progresser.</p>
    <h2>Ce Que Je Recherche</h2>
    <p>
      Je suis en constante quête d'opportunités pour améliorer mes compétences et contribuer à des projets innovants. Si vous partagez la même passion pour le web et l'art du code, je serais ravi d'échanger et de collaborer ! N’hésitez pas à me contacter pour discuter de vos projets ou de vos idées.
    </p>

      <article>
        <h2>Compétences</h2>
        <skills-images />
      </article>

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
    padding-top: 3.8rem;
}


</style>
