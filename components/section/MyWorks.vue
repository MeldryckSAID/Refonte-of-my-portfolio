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
        paragraphe="Le défi 24 heures était un défi plein d'émotion incroyable et intrépide 
        Pourrez-vous comprendre toute cette complicité ? Le défi 24 heures est un événement phare du département MMI Montbéliard ..."
        image="/png/24h.png"
      />
    </div>
    <div class="section_travaux--2">
      <MyCard
        id="2"
        paragraphe="Le défi 24 heures était un défi plein d'émotion incroyable et intrépide 
        Pourrez-vous comprendre toute cette complicité ? Le défi 24 heures est un événement phare du département MMI Montbéliard ..."
        image="/png/rosace.png"
        :isReversed="true"
      />
      <MyWorksAnim2 class="visu2" />
    </div>
    <div class="section_travaux--2">
      <MyWorksAnim2 :isReversed="true" class="visu2" />
      <MyCard
        id="2"
        paragraphe="Le défi 24 heures était un défi plein d'émotion incroyable et intrépide 
        Pourrez-vous comprendre toute cette complicité ? Le défi 24 heures est un événement phare du département MMI Montbéliard ..."
        image="/png/T2M.png"
        :isReversed="false"
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
