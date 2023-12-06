<template>
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">Descriptif</h4>
    </MyTitle>
  </div>
  <div class="descriptif">
    <div class="img__descriptif">
      <img src="/png/24H/Logo_24_blue.png" alt="Logo du 24H" />
      <img src="/png/24H/Logo_24_white.png" alt="Logo du 24H variant" />
    </div>

    <div class="text__descriptif">
      <MyLineAnim1 />
      <p class="text">
        Le défi 24 heures était une aventure pleine d'émotions incroyables et
        intrépides, destinée aux étudiants les plus audacieux et studieux de
        notre formation. Cet événement majeur du département MMI Montbéliard
        rassemble toutes les promotions actuelles de la formation. À l'occasion
        des 25 ans du département, il a été exceptionnellement ouvert aux
        anciens, leur offrant l'opportunité de revivre les années de leur
        jeunesse.
      </p>
      <MyLineAnim2 class="invisible" />
    </div>
  </div>
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">Univers</h4>
    </MyTitle>
  </div>
  <div class="mood">
    <MyWorksAnim2 class="visu1" />
    <img src="/png/24H/Moodboard24.png" alt="Moodboard du projets" />
    <MyWorksAnim2 class="visu2" />
  </div>
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">L'harmonie</h4>
    </MyTitle>
  </div>
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
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">Les technologies utilisées</h4>
    </MyTitle>
  </div>
  <div class="tech">
    <MyTech name="ai" class="tech-item1" />
    <MyTech name="html" class="tech-item2" />
    <MyTech name="css" class="tech-item3" />
    <MyTech name="firebase" class="tech-item4" />
    <MyTech name="vue" class="tech-item5" />
    <MyTech name="js" class="tech-item6" />
    <MyTech name="figma" class="tech-item7" />
    <MyTech name="tail" class="tech-item8" />
    <MyIcon name="gitn" class="tech-item9" />
  </div>
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">Une petite visite ?</h4>
    </MyTitle>
  </div>

  <div class="visite">
    <MyVisite24MaquettePc>Visiter la maquette pc</MyVisite24MaquettePc>
    <MyVisite24MaquetteM>Visiter la maquette mobile</MyVisite24MaquetteM>
    <MyVisite24>Visiter le site</MyVisite24>
    <MyGit24 />
  </div>
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
  align-items: center;
}
.text {
  font-family: $secondary-font;
  text-align: left;
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
  grid-template-rows: repeat(3, 1fr);
  gap: 25px;
  justify-items: center;
}
.introT {
  margin-left: 5%;
}
.invisible {
  opacity: 0;
  
}
</style>
