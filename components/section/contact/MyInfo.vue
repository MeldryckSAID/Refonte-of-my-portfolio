<template>
  <div class="section__info">
    <div class="info__text">
      <p>
        Intéressé(e) par une collaboration avec un jeune web développeur et
        webdesigner ? N'hésitez pas à m'envoyer un message ! Votre projet est
        important pour moi. Vous pouvez également me retrouver sur :
      </p>
      <p>
        Ou contactez-moi directement au 
        <a class="link" href="tel:+33772428966">+33 7 72 42 89 66</a>
      </p>
    </div>
    <div class="info__social">
      <a href="https://github.com/MeldryckSAID"
        ><MyIcon name="gitn"></MyIcon
      ></a>
      <a href="https://www.linkedin.com/in/meldryck-said/">
        <MyIcon name="linkedinn"></MyIcon
      ></a>
      <a href="/CV_MELDRYCK_SAID.pdf" download>
        <Mybutton> Mon Cv juste ici</Mybutton></a
      >
    </div>
  </div>
</template>
<style lang="scss">
.section__info {
  display: flex;
  justify-content: space-around;
  .info__text {
    p {
      width: 539px;
      font-family: $primary-font;
      font-size: 20px;
    }
  }
  .info__social {
    display: flex;
    gap: 30px;
    a {
      width: fit-content;
    }
  }
}
</style>

<script setup></script>
