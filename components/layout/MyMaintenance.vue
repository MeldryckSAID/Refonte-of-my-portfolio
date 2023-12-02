<template>
  <div class="maintenance-page">
    <div class="chill">
      <MyLineAnim3 class="anim3" />
      <MyLogo size="regular" />
      <MyLineAnim3 class="reverse anim3" />
    </div>

    <MyTitle el="h2" size="large"><h2>Site en maintenance</h2></MyTitle>

    <p>
      Je travaille actuellement sur cette portions du site. Le contenu n'est pas
      encore disponible. Veuillez consulter le site en version PC .
    </p>
    <p>A très vite</p>
  </div>
</template>

<style lang="scss" scoped>
.maintenance-page {
  text-align: center;
  margin: 20% auto;
  display: flex;
  align-items: center;
  flex-direction: column;
  .chill {
    display: flex;
    justify-content: space-evenly;
    .reverse {
      transform: scaleX(-1);
    }
  }
}


</style>
