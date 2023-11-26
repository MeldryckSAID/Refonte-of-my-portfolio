<template>
  <div>
    <MyLineAnim1 />
    <div class="present">
      <h2 class="present__Title">Qui suis je ?</h2>
      <p class="present__text">
        Pour l’instants un étudiant de Troisièmes année du département MMI
        Montbéliard et anciens Président du Bureau des Etudiants (BDE) au sein
        de cette formation j’ai pu acquérir plusieurs compétence et mon
        portefolio en ai la preuve.
      </p>
    </div>
    <MyLineAnim2 />
  </div>
</template>
<script setup></script>
<style lang="scss">
.present {
  display: flex;
  flex-direction: colum;
  &__Title {
    font-family: $primary-font;
  }
  &__text {
    font-family: $secondary-font;
  }
}
</style>
