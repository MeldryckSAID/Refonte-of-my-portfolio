<template>
  <MyTitle el="h4" size="large">
    <h4 class="intro__section">Descriptif</h4>
  </MyTitle>
  <div class="descriptif">
    <div class="img__descriptif">
      <MyLineAnim3 />
      <img
        src="/png/Expo.png"
        alt="Logo De l'exposition artistique de MMI Montbeliard"
      />
      <MyLineAnim3 class="reverse" />
    </div>
    <div class="text__descriptif">
      <MyLineAnim1 />
      <p class="text">
        La première édition de l'exposition au sein du département MMI de
        Montbéliard a été organisée dans le but de déconstruire le stéréotype du
        'geek'. En effet nos camarades étudiants etudies différents matiere avec
        3 poles premiers chacun on un aspects bien a eux "La Communication", "Le
        Dévelloppement Web" et le "Design numérique" Cet événement artistique a
        été conçu pour démontrer que les compétences de nos étudiants ne se
        limitent pas qu'a l'informatique. Nous vous invitons à découvrir par
        vous-même la diversité des talents présentés lors de cette exposition.
      </p>
      <MyLineAnim2 />
    </div>
  </div>
  <MyTitle el="h4" size="large">
    <h4 class="intro__section">Univers</h4>
  </MyTitle>
  <div class="mood">
    <MyWorksAnim2 class="visu1" />
    <img
      class="mood-img"
      src="/png/T2M/MoodboardMMi.png"
      alt="Moodboard du projets"
    />
    <MyWorksAnim2 class="visu2" />
  </div>

  <MyTitle el="h4" size="large">
    <h4 class="intro__section">L'harmonie</h4>
  </MyTitle>

  <div class="img__harmonie">
    <img
      class="cover"
      src="/png/T2M/Guide.png"
      alt="Guide de style de l'exposition Artisitique de MMI MONTbéliard"
    />
    <img class="cover" src="/png/T2M/Logo.png" alt="Le logo et son concept" />
    <img
      class="cover"
      src="/png/T2M/Couleurs.png"
      alt="Les couleurs choisi pour aborder notre thématique"
    />
    <img
      class="cover"
      src="/png/T2M/Typographie.png"
      alt="Typographie pour sublimer notre style"
    />
    <img
      class="cover"
      src="/png/T2M/Styles.png"
      alt="Les styles génériques qui seront utilisé pour le site"
    />
  </div>

  <MyTitle el="h4" size="large">
    <h4 class="intro__section">Les technologies utilisées</h4>
  </MyTitle>

  <div class="tech">
    <MyTech name="ai" class="tech-item2" />
    <MyTech name="ap" class="tech-item3" />
    <MyTech name="figma" class="tech-item4" />
  </div>
  <MyTitle el="h4" size="large">
    <h4 class="intro__section">Les technologies envisager</h4>
  </MyTitle>

  <div class="tech">
    <MyTech name="html" class="tech-item1" />
    <MyTech name="css" class="tech-item2" />
    <MyTech name="three" class="tech-item3" />
    <MyTech name="nuxt" class="tech-item4" />
    <MyTech name="js" class="tech-item7" />
    <MyTech name="vercel" class="tech-item8" />
  </div>

  <MyTitle el="h4" size="large">
    <h4 class="intro__section">Une petite visite ?</h4>
  </MyTitle>
  <div class="visite">
    <MyVisiteExpo>Visiter la maquette pc</MyVisiteExpo>
    <MyVisiteExpoM>Visiter la maquette mobile</MyVisiteExpoM>
  </div>
</template>

<script setup scoped></script>
<style lang="scss">
.img__descriptif {
  margin-bottom: 5%;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  .reverse {
    transform: scaleX(-1);
  }
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
.visite {
  display: flex;
  justify-content: space-around;
}
</style>
