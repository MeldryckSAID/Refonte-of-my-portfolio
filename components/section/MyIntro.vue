<template>
  <div class="intro">
    <MyWavesAnim class="intro__waves" />
    <MyLogo class="intro__logo" />
    <MySoundAnim class="intro__sound" />
  </div>
</template>
<script setup></script>
<style lang="scss">
.intro {
  &__logo {
    width: 369px;
    z-index: 1;
    
  }
  &__waves {
    position: relative;
    width: max-content;
    z-index: 0;
  }
  &__sound {
    position: relative;
    width: max-content;
    z-index: 0;
  }
}
</style>
