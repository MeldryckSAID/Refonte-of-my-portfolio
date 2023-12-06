<template>
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">Descriptif</h4>
    </MyTitle>
  </div>
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
        'geek'. En effet, nos camarades étudiants étudient différentes matières
        avec trois pôles distincts : "La Communication", "Le Développement Web"
        et le "Design numérique". Cet événement artistique a été conçu pour
        démontrer que les compétences de nos étudiants ne se limitent pas qu'à
        l'informatique. Nous vous invitons à découvrir par vous-même la
        diversité des talents présentés lors de cette exposition.
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
      src="/png/Expo/MoodboardMMi.png"
      alt="Moodboard du projets"
    />
    <MyWorksAnim2 class="visu2" />
  </div>
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">L'harmonie</h4>
    </MyTitle>
  </div>
  <div class="img__harmonie">
    <img
      class="cover"
      src="/png/Expo/Guide.png"
      alt="Guide de style de l'exposition Artisitique de MMI MONTbéliard"
    />
    <img class="cover" src="/png/Expo/Logo.png" alt="Le logo et son concept" />
    <img
      class="cover"
      src="/png/Expo/Couleurs.png"
      alt="Les couleurs choisi pour aborder notre thématique"
    />
    <img
      class="cover"
      src="/png/Expo/Typographie.png"
      alt="Typographie pour sublimer notre style"
    />
    <img
      class="cover"
      src="/png/Expo/Styles.png"
      alt="Les styles génériques qui seront utilisé pour le site"
    />
  </div>
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">Les technologies utilisées</h4>
    </MyTitle>
  </div>
  <div class="tech">
    <MyTech name="ai" class="tech-item2" />
    <MyTech name="ap" class="tech-item3" />
    <MyTech name="figma" class="tech-item4" />
  </div>
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">Les technologies envisager</h4>
    </MyTitle>
  </div>
  <div class="tech">
    <MyTech name="html" class="tech-item1" />
    <MyTech name="css" class="tech-item2" />
    <MyTech name="three" class="tech-item3" />
    <MyTech name="nuxt" class="tech-item4" />
    <MyTech name="js" class="tech-item7" />
    <MyTech name="vercel" class="tech-item8" />
    <MyIcon name="gitn" />
  </div>
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">Une petite visite ?</h4>
    </MyTitle>
  </div>
  <div class="visite">
    <MyVisiteExpo>Visiter la maquette pc</MyVisiteExpo>
    <MyVisiteExpoM>Visiter la maquette mobile</MyVisiteExpoM>
  </div>
</template>

<script setup></script>
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
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(2, 1fr); /* Trois lignes maintenant */
  gap: 20px;
  justify-items: center;
}
.visite {
  display: flex;
  justify-content: space-around;
}
</style>
