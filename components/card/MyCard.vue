<template>
  <div class="card">
    <div class="card__content" :class="{ '--reversed': isReversed }">
      <img class="card__image" :src="image" alt="" />
      <div class="card__text">
        <p class="">{{ paragraphe }}</p>
        <Mybutton>En savoir plus</Mybutton>
      </div>
    </div>
  </div>
</template>
<script setup>
defineProps({
  id: Number,
  paragraphe: String,
  image: String,
  isReversed: Boolean,
});
</script>
<style lang="scss">
.card {
  width: 1012px;

  margin: 10px;
  display: flex;

  &__content {
    display: flex;
    border: 10px solid black;
    &.--reversed {
      flex-direction: row-reverse;
    }
    .card__image {
      width: fit-content;
    }
    .card__text {
      line-height: 1.5;
      padding: 3%;
      font-family: $primary-font;
      text-align: justify;
      display: flex;
      align-items: center;
      display: flex;
      flex-direction: column;
      justify-content: center;
    }
  }
}
</style>
