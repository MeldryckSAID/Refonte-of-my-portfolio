<template>
  <div class="intro_contact">
    <MySoundAnim class="intro_contact__sound " />
    <MyTitle el="h2" size="medium">
      <h2 class="intro__title">Contact Me</h2>
    </MyTitle>
    <MySoundAnim class="intro_contact__sound2" />
  </div>
</template>
<script setup></script>
<style lang="scss">
.intro_contact {
  display: flex;
  justify-content: space-around;
  align-items: center;

  &__sound {
    position: relative;
    width: min-content;
    z-index: 0;
    transform: scaleX(-1);
  }

  &__sound2 {
    right: 0;
  }
}
</style>
