<template>
  <div class="intro_travaux">
    <MyWorksLineTAnim class="intro_travaux__line" />

    <MyTitle el="h2" size="medium">
      <h2 class="intro__title"><slot></slot></h2>
    </MyTitle>
    <div class="line__rigth">
      <MyWorksLineTAnim class="intro_travaux__line2" />
    </div>
  </div>
</template>
<script setup></script>
<style lang="scss">
.intro_travaux {
  .intro__title {
    display: flex;
    justify-content: center;
  }
  &__line {
    position: relative;
    width: min-content;
    z-index: 0;
    top: 0;
  }
  .line__rigth {
    display: flex;
    justify-content: end;
    .intro_travaux__line2 {
      transform: scaleY(-1);
      transform: scaleX(1);
    }
  }
}
</style>
