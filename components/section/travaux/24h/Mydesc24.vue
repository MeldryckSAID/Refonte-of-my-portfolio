<template>
  <MyTitle el="h4" size="large">
    <h4 class="intro__section">Descriptif</h4>
  </MyTitle>
  <div class="descriptif">
    <div class="img__descriptif">
      <img src="/png/24H/24h arr.png" alt="Logo du 24H" />
      <img src="/png/24H/24h w.png" alt="Logo du 24H variant" />
    </div>
    <div class="text__descriptif">
      <p class="text">
        Le défi 24 heures était un défi plein d'émotion incroyable et intrépide
        fait pour les plus intépides , les plus studieux des étudiants de notre
        formation. Le défi 24 heures est un événement phare du département MMI
        Montbéliard qui reuni toutes les promotions présente de la formations, a
        l'occasion des 25 ans du départements cette fois ci il a été ouvert aux
        anciens leurs permettants de revenir vivre les années de leurs
        jeunesses.
      </p>
    </div>
  </div>
  <MyTitle el="h4" size="large">
    <h4 class="intro__section">Univers</h4>
  </MyTitle>
  <div class="mood">
    <MyWorksAnim2 class="visu1" />
    <img src="/png/24H/Moodboard24.png" alt="Moodboard du projets" />
    <MyWorksAnim2 class="visu2" />
  </div>

  <MyTitle el="h4" size="large">
    <h4 class="intro__section">L'harmonie</h4>
  </MyTitle>

  <div class="img__harmonie">
    <img class="cover" src="/png/24H/Couverture.png" alt="Logo du 24H" />
    <img class="cover" src="/png/24H/Logo24.png" alt="Logo du 24H variant" />
    <img class="cover" src="/png/24H/Couleurs.png" alt="Logo du 24H variant" />
    <img
      class="cover"
      src="/png/24H/Typographie.png"
      alt="Logo du 24H variant"
    />
  </div>

  <MyTitle el="h4" size="large">
    <h4 class="intro__section">Les technologies utilisées</h4>
  </MyTitle>

  <div class="tech">
    <MyTech name="ai" class="tech-item1" />
    <MyTech name="html" class="tech-item2" />
    <MyTech name="css" class="tech-item3" />
    <MyTech name="firebase" class="tech-item4" />
    <MyTech name="vue" class="tech-item5" />
    <MyTech name="js" class="tech-item6" />
    <MyTech name="figma" class="tech-item7" />
    <MyTech name="tail" class="tech-item8" />
  </div>

  <MyTitle el="h4" size="large">
    <h4 class="intro__section">Une petite visite ?</h4>
  </MyTitle>
  <MyVisite24/>
</template>

<script setup></script>
<style lang="scss">
.img__descriptif {
  margin-bottom: 5%;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
}
.mood {
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.visu1 {
  transform: scaleX(-1);
}
.text__descriptif {
  display: flex;
  justify-content: center;
}
.text {
  font-family: $secondary-font;
  text-align: center;
  width: 625px;
}
.descriptif {
  margin-bottom: 5%;
}
.img__harmonie {
  display: flex;
  flex-direction: column;
  .cover {
    width: 100%;
    margin: 0;
  }
}
.tech {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-template-rows: repeat(2, 1fr); /* Trois lignes maintenant */
  gap: 10px;
  justify-items: center;
}
</style>
