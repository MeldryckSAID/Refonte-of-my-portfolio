<template>
  <div class="section__presentation">
    <MyLineAnim1 />
    <div class="present">
      <MyTitle el="h2" size="medieum">
        <h2 class="intro__title">Bienvenue</h2>
      </MyTitle>
      <h2 class="present__Title">Qui suis je ?</h2>
      <p class="present__text">
        Pour l’instant un étudiant de Troisièmes années du département MMI
        Montbéliard et anciens Président du Bureau des Etudiants (BDE) au sein
        de cette formation j’ai pu acquérir plusieurs compétences et mon
        portfolio en est une preuve.
      </p>
    </div>
    <MyLineAnim2 />
  </div>
</template>
<script setup></script>
<style lang="scss">
.section__presentation {
  display: flex;
  justify-content: center;
  align-items: center;
}
.present {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 625px;
  &__Title {
    font-family: $primary-font;
  }
  &__text {
    font-family: $secondary-font;
  }
}
</style>
