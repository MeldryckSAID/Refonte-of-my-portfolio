<template>
  <div class="section_travaux">
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
      <div class="section_travaux--4">
        <MyCard
          id="2"
          titre="Osaka"
          paragraphe="Comment convaincre les fidèles comme les nouveaux visiteurs de venir à l’expo universelle 2025 ?
          Par conséquences réussir à attirer l’attention des visiteurs en créant un événement qui tisse 
          un lien entre les humains, la nature et la technologie. ..."
          image="/png/rosace.png"
          :isReversed="false"
          buttonLink="/Projets/osaka"
        />
      </div>
      <div class="section_travaux--5">
        <MyCard
          id="2"
          titre="Time2Match"
          paragraphe="Lors de ce projet nous avions pour ambitions de connecter les sportifs et 
          le sport organiser c'est ce que 
          nous avons fait en leurs apportant Time2match qui leur permettront de mieux 
          s'organiser pour leurs séances de sport collectif"
          image="/png/T2M.png"
          :isReversed="true"
          buttonLink="/Projets/T2M"
        />
      </div>
    </div>
    <div class="sous">
      <MyWorksLineWhithScrollAnim />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.section_travaux {
  display: flex;
  align-items: center;
  flex-direction: column;
}
.works {
  position: relative;
  z-index: 2;
  margin-top: 10%;
  margin-bottom: 10%;
}

.sous {
  z-index: 1;
  position: absolute;
  margin-top: 5%;
  margin-bottom: 10%;
}
</style>

<script setup></script>
