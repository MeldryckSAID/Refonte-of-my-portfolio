<template>
  <div class="section_travaux">
    <div class="works">
      <div class="section_travaux--1">
        <MyCard
          :id="1"
          titre="MMI Expo"
          paragraphe="La première édition d'une exposition artistique au Département MMI de Montbéliard vise à déconstruire le stéréotype du 'geek'.Cet événement énigmatique a été  conçu pour révéler, de manière significative , les compétences artistiques dissimulées. Découvrez  les compétences artistiques de nos étudiants lors de cet événement unique et intrigant."
          image="/png/Expo.png"
          :isReversed="true"
          buttonLink="/Projets/Expo"
        />
      </div>
      <div class="section_travaux--2">
        <MyCard
          :id="2"
          titre="Le défi 24h"
          paragraphe="Le défi des 24 heures était une expérience intense et audacieuse, pleine d'émotions. Pourrez-vous ressentir toute cette complicité ? Cet événement emblématique fait partie intégrante du département MMI Montbéliard."
          image="/png/24h.png"
          buttonLink="/Projets/24h"
        />
      </div>
      <div class="section_travaux--3">
        <MyCard
          :id="3"
          titre="MMI Montbéliard x International"
          paragraphe="Le département MMI Montbéliard vous offre l'opportunité de découvrir l'étranger pendant un semestre entier. Laissez-nous vous montrer comment vous serez convaincu"
          image="/png/mobile.png"
          :isReversed="true"
          buttonLink="/Projets/mobile"
        />
      </div>
      <div class="section_travaux--4">
        <MyCard
          :id="4"
          titre="Osaka"
          paragraphe="Comment convaincre aussi bien les fidèles que les nouveaux visiteurs de participer à l'exposition universelle 2025 ? Réussissons à attirer l'attention des visiteurs en créant un événement qui tisse des liens entre les humains, la nature et la technologie"
          image="/png/rosace.png"
          :isReversed="false"
          buttonLink="/Projets/osaka"
        />
      </div>
      <div class="section_travaux--5">
        <MyCard
          :id="5"
          titre="Time2Match"
          paragraphe="Dans le cadre de ce projet, notre ambition était de connecter les sportifs au sport organisé. C'est précisément ce que nous avons réalisé en introduisant Time2match, qui leur permettra de mieux organiser leurs séances de sport collectif."
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
