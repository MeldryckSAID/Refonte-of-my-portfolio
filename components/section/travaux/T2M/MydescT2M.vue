<template>
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">Descriptif</h4>
    </MyTitle>
  </div>
  <div class="descriptif">
    <div class="img__descriptif">
      <img src="/png/T2M/T2M_logo.webp" alt="Logo du T2M" />
    </div>
    <div class="text__descriptif">
      <MyLineAnim1 />
      <p class="text">
        Lors de ce projet, notre ambition était de renforcer la connexion entre
        les sportifs et le sport organisé, en mettant en place Time2match. Cette
        plateforme novatrice a été conçue pour offrir aux amateurs de sport
        collectif une solution complète. Elle facilite non seulement
        l'organisation de leurs séances, mais favorise également la cohésion au
        sein des équipes. Grâce à Time2match, les sportifs peuvent planifier
        efficacement leurs sessions de sport collectif, renforçant ainsi
        l'esprit d'équipe et l'expérience sportive collective.
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
    <img
      class="mood-img"
      src="/png/T2M/Moodboard.webp"
      alt="Moodboard du projet Time2Match"
    />
    <MyWorksAnim2 class="visu2" />
  </div>
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">L'harmonie</h4>
    </MyTitle>
  </div>

  <div class="img__harmonie">
    <img class="cover" src="/png/T2M/Couverture.webp" alt="Logo du T2M" />
    <img
      class="cover"
      src="/png/T2M/Typographies.webp"
      alt="Logo du T2M variant"
    />
    <img class="cover" src="/png/T2M/Couleurs.webp" alt="Logo du T2M variant" />
  </div>

  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">Les technologies utilisées</h4>
    </MyTitle>
  </div>

  <div class="tech">
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
    <MyVisiteT2MMaquettePc>Visiter la maquette pc</MyVisiteT2MMaquettePc>
    <MyVisiteT2M>Visiter le site</MyVisiteT2M>
    <MyGitT2m />
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
  &-img {
    width: 50%;
  }
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
  grid-template-rows: repeat(2, 1fr); /* Trois lignes maintenant */
  gap: 10px;
  justify-items: center;
}

.invisible {
  opacity: 0;
  svg {
    opacity: 0;
  }
}
</style>
