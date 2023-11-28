<template>
  <div class="section_travaux">
    <div class="works">
      <div class="section_travaux--1">
        <MyCard
          id="1"
          paragraphe="Le défi 24 heures était un défi plein d'émotion incroyable et intrépide 
        Pourrez-vous comprendre toute cette complicité ? Le défi 24 heures est un événement phare du département MMI Montbéliard ..."
          image="/png/24h.png"
        />
      </div>
      <div class="section_travaux--2">
        <MyCard
          id="2"
          paragraphe="Comment convaincre les fidèles comme les nouveaux visiteurs de venir à l’expo universelle 2025 ?
          Par conséquences réussir à attirer l’attention des visiteurs en créant un événement qui tisse 
          un lien entre les humains, la nature et la technologie. ..."
          image="/png/rosace.png"
          :isReversed="true"
        />
      </div>
      <div class="section_travaux--3">
        <MyCard
          id="2"
          paragraphe="Lors de ce projet nous avions pour ambitions de connecter les sportifs et 
          le sport organiser c'est ce que 
          nous avons fait en leurs apportant Time2match qui leur permettront de mieux 
          s'organiser pour leurs séances de sport collectif"
          image="/png/T2M.png"
          :isReversed="false"
        />
      </div>
      <div class="section_travaux--4">
        <MyCard
          id="2"
          paragraphe="Le défi 24 heures était un défi plein d'émotion incroyable et intrépide 
        Pourrez-vous comprendre toute cette complicité ? Le défi 24 heures est un événement phare du département MMI Montbéliard ..."
          image="/png/expo.png"
          :isReversed="true"
        />
      </div>
      <div class="section_travaux--5">
        <MyCard
          id="2"
          paragraphe="Le défi 24 heures était un défi plein d'émotion incroyable et intrépide 
        Pourrez-vous comprendre toute cette complicité ? Le défi 24 heures est un événement phare du département MMI Montbéliard ..."
          image="/png/T2M.png"
          :isReversed="false"
        />
      </div>
    </div>
    <div class="sous">
      <MyWorksLineWhithScrollAnim />
    </div>
  </div>
</template>

<style lang="scss">
.section_travaux {
  display: flex;
  align-items: center;
  flex-direction: column;
}
.works {
  position: absolute;
  z-index: 2;
}

.sous {
  z-index: 1;
  position: relative;
}
</style>

<script setup></script>
