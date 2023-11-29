<template>
  <div class="section_travaux">
    <div class="intro__title">
      <MyTitle el="h3" size="large">
        <h3 class="">Mes Travaux</h3>
      </MyTitle>
    </div>
    <div class="section_travaux--1">
      <MyWorksAnim1 class="visu1" />
      <MyCard
        id="1"
        titre="MMI Expo"
        paragraphe="La première édition de l'exposition  au sein du 
          département MMI de Montbéliard a été organisée dans le but de déconstruire le 
          stéréotype du 'geek'. Cet événement artistique a été conçu pour démontrer que les 
          compétences des étudiants ne se limitent pas à l'informatique. Nous vous invitons à découvrir par vous-même 
          la diversité des talents présentés lors de cette exposition."
        image="/png/expo.png"
        :isReversed="true"
        buttonLink="/Projets/Expo"
      />
    </div>
    <div class="section_travaux--2">
      <MyCard
        id="2"
        titre="Le défit 24h"
        paragraphe="Le défi 24 heures était un défi plein d'émotion incroyable et intrépide 
        Pourrez-vous comprendre toute cette complicité ? Le défi 24 heures est un événement phare du département MMI Montbéliard ..."
        image="/png/24h.png"
        buttonLink="/Projets/24h"
      />
      <MyWorksAnim2 class="visu2" />
    </div>
    <div class="section_travaux--2">
      <MyWorksAnim2 :isReversed="true" class="visu2" />
      <MyCard
        id="3"
        titre="MMI Montbéliard x International"
        paragraphe="Le département MMI Montbéliard vous offre la possibilité d'aler d'écouvrir l'étranger pendants tout un semestre 
          laisser nous vous montrez comment vous allez etre convaincu..."
        image="/png/mobile.png"
        :isReversed="true"
        buttonLink="/Projets/mobile"
      />
      />
    </div>
  </div>
</template>

<style lang="scss">
.intro__title {
  display: flex;
  justify-content: center;
}

.section_travaux {
  display: flex;
  align-items: center;
  flex-direction: column;

  .section_travaux--1 {
    display: flex;
    align-items: stretch;
  }

  .visu1 {
    margin-top: -145px;
    margin-left: 25px;
    z-index: 1;
  }
  .section_travaux--2 {
    display: flex;
    align-items: stretch;
  }

  .visu2 {
    z-index: 1;
  }
}
</style>

<script setup></script>
