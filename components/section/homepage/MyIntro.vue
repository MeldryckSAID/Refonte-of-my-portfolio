<template>
  <div class="intro">
    <MyWavesAnim class="intro__waves" />
    <MyLogo size="big" class="intro__logo" />
    <MyWavesAnim class="intro__wave2" />
  </div>
</template>
<script setup></script>
<style lang="scss">
.intro {
  display: flex;
  justify-content: space-between;
  align-items: center;
  &__logo {
    width: 269px;
    z-index: 1;
  }
  &__waves {
    position: relative;
    width: min-content;
    z-index: 0;
  }
  &__wave2 {
    transform: scaleX(-1); 
    right: 0;
  }
}
</style>
