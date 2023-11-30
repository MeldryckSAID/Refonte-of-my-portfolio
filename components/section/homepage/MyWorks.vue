<template>
  <div class="section_travaux">
    <div class="intro__title">
      <MyTitle el="h3" size="large">
        <h3 class="">Mes Travaux</h3>
      </MyTitle>
    </div>
    <div class="travaux__grid">
      <div>
        <MyWorksAnim2 :isReversed="true" class="visu1" />
        <MyWorksAnim2 :isReversed="true" class="visu2" />
        <MyWorksAnim2 :isReversed="true" class="visu1" />
      </div>
      <div class="works">
        <div class="section_travaux--1">
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
        </div>
        <div class="section_travaux--3">
          <MyCard
            id="3"
            titre="MMI Montbéliard x International"
            paragraphe="Le département MMI Montbéliard vous offre la possibilité d'aler d'écouvrir l'étranger pendants tout un semestre 
          laisser nous vous montrez comment vous allez etre convaincu..."
            image="/png/mobile.png"
            :isReversed="true"
            buttonLink="/Projets/mobile"
          />
        </div>
      </div>
      <div>
        <MyWorksAnim2 :isReversed="true" class="visu2" />
        <MyWorksAnim2 :isReversed="true" class="visu1" />
        <MyWorksAnim2 :isReversed="true" class="visu2" />
      </div>
    </div>
    <div class="more">
      <Mybutton to="/Projets">Voir tout les projet</Mybutton>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.more,
.intro__title {
  display: flex;
  justify-content: center;
}
.more{
  margin-bottom: 20px;
}
.travaux__grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  .visu1 {
    z-index: 1;
    transform: scaleX(1);
  }
  .visu2 {
    z-index: 1;
    transform: scaleX(-1);
  }
}
</style>

<script setup></script>
