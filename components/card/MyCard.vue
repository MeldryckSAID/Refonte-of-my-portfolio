<template>
  <div class="card__content" :class="{ '--reversed': isReversed }">
    <img class="card__image" :src="image" alt="" />
    <div class="card__text">
      <MyTitle el="h5" size="medium">{{ titre }}</MyTitle>
      <p class="text">{{ paragraphe }}</p>
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
  display: flex;
  border: 5px solid black;
  background: white;
  margin-bottom: 5rem;
  &.--reversed {
    flex-direction: row-reverse;
  }
  .card__image {
    width: fit-content;
  }
  .card__text {
    line-height: 1.5;
    padding-left: 20px;
    padding-right: 20px;
    font-family: $secondary-font;
    text-align: center;
  }
}
</style>
