<template>
  <div class="section__presentation">
    <MyLineAnim1 />
    <div class="present">
      <MyTypewriter />

      <p class="present__text">
        Actuellement étudiant en BUT (Brevet Universitaire de Technologie), en
        troisième année du département Métiers du Multimédia et de l'Internet
        (MMI) à Montbéliard, avec un parcours en développement web et
        dispositifs interactifs, et ancien Président du Bureau des Étudiants
        (BDE) au sein de cette formation, cette expérience m'a permis d'acquérir
        diverses compétences à travers les trois pôles : communication, design
        et développement, comme en témoigne mon portfolio.
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
  gap: 40px;
  &__Title {
    font-family: $primary-font;
  }
  &__text {
    font-family: $secondary-font;
  }
}
</style>
