<template>
  <div class="card">
    <div class="card__content">
      <img class="card__image" :src="image" alt="" />
      <div class="card__text">
        <p class="">{{ paragraphe }}</p>
      </div>
    </div>
  </div>
</template>
<script setup>
defineProps({
  id: Number,
  paragraphe: String,
  image: String,
});
</script>
<style lang="scss">
.card {
  border: 20px solid black;
  background: red;
  &__content {
    background: aqua;
    display: flex;
  }
}
</style>
