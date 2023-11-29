<template>
  <RouterLink class="contact" :to="`/Contact`">
    <div class="">
      <div class="contact__content">
        <MyLogo size="small" />
        <MyTitle el="h3" size="large">
          <h2 class="contact__title">Contactez Moi</h2>
        </MyTitle>
        <MyLogo size="small" />
      </div>
    </div>
  </RouterLink>
</template>
<style lang="scss">
.contact {
  display: flex;
  justify-content: center;
  margin-top: 10%;
  text-decoration: none;
  &__content {
    background-color: $D;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 828px;
    gap: 30px;
    border-radius: 26px;
    .contact__title {
      color: $L;
    }
  }
}
</style>
<script setup></script>
