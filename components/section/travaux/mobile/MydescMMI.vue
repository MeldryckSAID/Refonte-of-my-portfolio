<template>
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">Descriptif</h4>
    </MyTitle>
  </div>
  <div class="descriptif">
    <div class="img__descriptif">
      <img src="/png/mobile/Mobile_blanc.png" alt="Logo du 24H" />
      <img src="/png/mobile/Mobile_noir.png" alt="Logo du 24H variant" />
    </div>
    <div class="text__descriptif">
      <MyLineAnim1 />
      <p class="text">
        Notre travail a commencé par une analyse de la stratégie de
        communication existante du département et la mise en œuvre d'un audit
        SEO. Cet audit a été suivi de recommandations stratégiques et d'une
        nouvelle stratégie de médias sociaux. Suite à ce travail de
        communication, nous avons pu aborder la partie design du projet, avec
        notamment la refonte du logo de la variante internationale de MMI, la
        création d'une identité graphique (web et print), d'une charte graphique
        sous forme de brandboard (web et print), d'affiches et de cartes
        postales (web et print), et d'un wireframe de la page d'accueil du site
        web pour proposer les nouvelles fonctionnalités envisagées suite à nos
        études de communication. Nous sommes ensuite passés à la production de
        contenu, plus précisément de posts visuels et de vidéos pour nos
        différents réseaux sociaux. Pour les vidéos, nous avons dû les tourner,
        les doubler et les monter. Enfin, nous avons pu présenter nos différents
        contenus sur Behance, avec des explications pour justifier nos choix
        pour chacun d'entre eux. Traduit avec DeepL.com (version gratuite)
      </p>
      <MyLineAnim2 />
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
      src="/png/mobile/Affiche_v1.jpg"
      alt="Premier design de l'affiche MMI Montbéliard intenational "
    />
    <img
      class="mood-img"
      src="/png/mobile/Affiche_v2.png"
      alt="Second design de l'affiche MMI Montbéliard intenational "
    />
    <MyWorksAnim2 class="visu2" />
  </div>
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">D'autres éléments</h4>
    </MyTitle>
  </div>

  <div class="img__harmonie">
    <img
      class="cover"
      src="/png/mobile/Carte_Postale_v1-1.png"
      alt="Logo du 24H"
    />
    <img
      class="cover"
      src="/png/mobile/Carte_Postale_v1-2.png"
      alt="Logo du 24H variant"
    />
  </div>
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">Les technologies utilisées</h4>
    </MyTitle>
  </div>
  <div class="techno__use">
    <MyTech name="ai" class="tech-item1" />
    <MyTech name="indi" class="tech-item2" />
    <MyTech name="figma" class="tech-item3" />
    <MyTech name="pr" class="tech-item4" />
    <MyTech name="davinci" class="tech-item4" />
  </div>

  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">Une petite visite ?</h4>
    </MyTitle>
  </div>

  <div class="visite">
    <MyVisiteMMI>Visiter sur behance</MyVisiteMMI>
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
    width: 20%;
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
  justify-content: space-around;
  flex-direction: row;
  .cover {
    width: 40%;
    margin: 0;
  }
}
.techno__use {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  gap: 10px;
  justify-items: center;
}
</style>
