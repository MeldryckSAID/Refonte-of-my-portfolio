<template>
  <div class="card__content" :class="{ '--reversed': isReversed }">
    <img class="card__image" :src="image" alt="" />
    <div class="card__text">
      <MyTitle el="h5" size="medium">{{ titre }}</MyTitle>
      <p class="">{{ paragraphe }}</p>
      <Mybutton :to="buttonLink"> En savoir plus </Mybutton>
    </div>
  </div>
</template>
<script setup>
defineProps({
  id: Number,
  paragraphe: String,
  titre: String,
  image: String,
  isReversed: Boolean,
  buttonLink: String,
});
</script>
<style lang="scss">
.card__content {
  width: 1012px;
  display: flex;
  //border: 5px solid black;
  border-radius: 14px;
  background: white;
  margin-bottom: 5rem;
  filter: drop-shadow(20px 22px 33.79999923706055px rgba(0, 0, 0, 0.3));
  &.--reversed {
    flex-direction: row-reverse;
    .card__image {
      width: fit-content;
      border-top-right-radius: 14px;
      border-bottom-right-radius: 14px;
      border-top-left-radius: 0px;
      border-bottom-left-radius: 0px;
    }
  }
  .card__image {
    width: fit-content;
    border-top-left-radius: 14px;
    border-bottom-left-radius: 14px;
  }
  .card__text {
    line-height: 1.5;
    padding-left: 20px;
    padding-right: 20px;
    font-family: $secondary-font;
    text-align: center;
    max-width: max-content;
  }
}
</style>
