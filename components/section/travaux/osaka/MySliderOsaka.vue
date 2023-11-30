<template>
  <div class="carrouselCards">
    <div class="iconFleche iconFleche-gauche" @click="showPreviousCard">
      <img src="/path/to/left-arrow.png" alt="Flèche gauche" />
    </div>
    <div class="iconFleche iconFleche-droit" @click="showNextCard">
      <img src="/path/to/right-arrow.png" alt="Flèche droite" />
    </div>

    <div class="carrouselCards__carrousel" ref="carrousel">
      <img v-for="card in donnees" src="/png/osaka/affiche/Affichev1.png" alt="Flèche droite"  />
      <img v-for="card in donnees" src="/png/osaka/affiche/Affichev2.png" alt="Flèche droite"  />
      <img v-for="card in donnees" src="/png/osaka/affiche/Affichev3.png" alt="Flèche droite"  />
      <img v-for="card in donnees" src="/png/osaka/affiche/Affichev4.png" alt="Flèche droite"  />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.carrouselCards {
  position: relative;
  width: 730px;

  .iconFleche {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    cursor: pointer;

    &-droit {
      right: 0;
      transform: translateX(50%);
    }

    &-gauche {
      left: 0;
      transform: translateX(-50%);
    }
  }

  &__carrousel {
    display: flex;
    flex-direction: row-reverse;
    overflow: hidden;
    max-width: 730px;
    min-width: 500px;
    box-shadow: 0px 0px 30px 0px rgba($D, 30%);
    border-radius: 35px;

    img {
      width: 100%;
      height: auto;
    }

    .active {
      transition: opacity 0.3s ease-in-out;
      opacity: 1;
    }
  }
}
</style>

<script setup>
import { ref } from "vue";

const donnees = [
  { id: 1, imageSrc: "/path/to/image1.jpg", altText: "Image 1" },
  { id: 2, imageSrc: "/path/to/image2.jpg", altText: "Image 2" },
  // Ajoutez autant d'objets que nécessaire
];

const activeCard = ref(donnees[0]);

const showNextCard = () => {
  const currentIndex = donnees.indexOf(activeCard.value);
  if (currentIndex < donnees.length - 1) {
    activeCard.value = donnees[currentIndex + 1];
  } else {
    activeCard.value = donnees[0];
  }
};

const showPreviousCard = () => {
  const currentIndex = donnees.indexOf(activeCard.value);
  if (currentIndex > 0) {
    activeCard.value = donnees[currentIndex - 1];
  } else {
    activeCard.value = donnees[donnees.length - 1];
  }
};
</script>
