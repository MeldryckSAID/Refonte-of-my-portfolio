<template>
  <div class="contact">
    <RouterLink class="contact__link" :to="`/Contact`">
      <div class="contact__link__content">
        <MyLogo size="small" />
        <MyTitle el="h4" size="medium">
          <h2 class="contact__title">Contactez Moi</h2>
        </MyTitle>
        <MyLogo size="small" />
      </div>
    </RouterLink>
  </div>
</template>
<style lang="scss">
.contact {
  display: flex;
  justify-content: center;
  

  .contact__link {
    margin-top: 0%;
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
}
</style>
<script setup></script>
