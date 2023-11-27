<template>
  <div class="section_travaux">
    <div class="intro__title">
      <MyTitle el="h3" size="large">
        <h3 class="">Mes Travaux</h3>
      </MyTitle>
    </div>
    <MyWorksAnim1/>
    <MyCard
      id="1"
      paragraphe="Le défi 24 heures était un défie plein d'émotion incroyable et intrépide 
    Pourrez-vous comprendre toute ça complicité  Le défi 24 heures est événement phares du département MMI Montbéliard ..."
      image="/png/24h.png"
    />
    <MyCard
      id="2"
      paragraphe="Le défi 24 heures était un défie plein d'émotion incroyable et intrépide 
    Pourrez-vous comprendre toute ça complicité  Le défi 24 heures est événement phares du département MMI Montbéliard ..."
      image="/png/rosace.png"
      :isReversed="true"
    />
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
}
</style>
<script setup></script>
