<template>
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">Descriptif</h4>
    </MyTitle>
  </div>
  <div class="descriptif">
    <div class="img__descriptif">
      <img
        src="/png/osaka/rosace_or.png"
        alt="Logo version or de la Campagne OASKA"
      />
      <img
        src="/png/osaka/rosace_original.png"
        alt="Logo Original de la Campagne OASKA"
      />
      <img
        src="/png/osaka/rosace_argent.png"
        alt="Logo version argent de la Campagne OASKAt"
      />
    </div>
    <div class="text__descriptif">
      <MyLineAnim1 />
      <p class="text">
        Comment convaincre les fidèles comme les nouveaux visiteurs de venir à
        l’expo universelle 2025 ? Par conséquences réussir à attirer l’attention
        des visiteurs en créant un événement qui tisse un lien entre les
        humains, la nature et la technologie. Le tout en offrant une nouvelle
        communication pour tout public qui conserve la fidélisation des
        visiteurs des années passées. Nous devions effectuer cette campagne sur
        des formats d'affiche et de carte postale.
      </p>
      <MyLineAnim2 />
    </div>
  </div>
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">L'harmonie</h4>
    </MyTitle>
  </div>
  <div class="mood">
    <MyWorksAnim2 class="visu1" />
    <div class="harmo">
      <p>
        La rosace symbolise la complexité de l’esprit humain ainsi que celle de
        la technologie. Les deux réunis crée une forme magnifique et intrigante
      </p>
      <img
        class="harmo-img"
        src="/png/osaka/couleur.png"
        alt="Logo version argent de la Campagne OASKAt"
      />
      <p class="">
        Argent : Il symbolise la technologie, l’IA
        <br />
        Vert : Il représente la nature
        <br />
        Rouge : Il représente l’humain (sang / chair) <br />
        Bleu : Il symbolise le lien entre les 3 éléments (eau pour nature,
        intelligence pour humain et technologie)
      </p>
    </div>
    <MyWorksAnim2 class="visu2" />
  </div>

  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">Résultat</h4>
    </MyTitle>
  </div>

  <div class="affiche">
    <MyTitle el="h5" size="medium">
      <h4 class="intro__section">Affiche</h4>
    </MyTitle>

    <div class="affiche-item">
      <img
        class="affiche-image"
        src="/png/osaka/affiche/Affichev1.png"
        alt="Logo version argent de la Campagne OASKAt"
      />
      <img
        class="affiche-image"
        src="/png/osaka/affiche/Affichev2.png"
        alt="Logo version argent de la Campagne OASKAt"
      />
      <img
        class="affiche-image"
        src="/png/osaka/affiche/Affichev3.png"
        alt="Logo version argent de la Campagne OASKAt"
      />
      <img
        class="affiche-image"
        src="/png/osaka/affiche/Affichev4.png"
        alt="Logo version argent de la Campagne OASKAt"
      />
    </div>
  </div>
  <div class="affiche">
    <MyTitle el="h5" size="medium">
      <h4 class="intro__section">Cartes Postales</h4>
    </MyTitle>

    <div class="affiche-item">
      <img
        class="affiche-image"
        src="/png/osaka/postale/A61.png"
        alt="Logo version argent de la Campagne OASKAt"
      />
      <img
        class="affiche-image"
        src="/png/osaka/postale/A65.png"
        alt="Logo version argent de la Campagne OASKAt"
      />
      <img
        class="affiche-image"
        src="/png/osaka/postale/A63.png"
        alt="Logo version argent de la Campagne OASKAt"
      />
      <img
        class="affiche-image"
        src="/png/osaka/postale/A64.png"
        alt="Logo version argent de la Campagne OASKAt"
      />
    </div>
  </div>
  <div class="introT">
    <MyTitle el="h4" size="large">
      <h4 class="intro__section">Les technologies utilisées</h4>
    </MyTitle>
  </div>
  <div class="tech">
    <MyTech name="ai" class="tech-item1" />
    <MyTech name="figma" class="tech-item3" />
  </div>
</template>

<script setup></script>
<style lang="scss" scoped>
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
  .harmo {
    display: flex;
    flex-direction: column;
    align-items: center;
    &-img {
      width: 70%;
    }
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
    width: 20%;
    margin: 0;
  }
}
.tech {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 10px;
  justify-items: center;
}
.affiche {
  display: flex;
  flex-direction: column;
  align-items: center;
  .affiche-item {
    display: flex;
    align-items: center;
    justify-content: space-around;
    img {
      width: 20%;
    }
  }
}
</style>
