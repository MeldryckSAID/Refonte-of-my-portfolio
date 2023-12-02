<template>
  <div class="footer__content">
    <RouterLink :to="`/`">
      <MyLogo size="regular" class="Logo_footer" />
    </RouterLink>
    <div class="footer-information">
      <div class="footer-social">
        <a href="https://github.com/MeldryckSAID"
          ><MyIcon fill="white" name="git"></MyIcon
        ></a>
        <a href="https://www.linkedin.com/in/meldryck-said/">
          <MyIcon fill="white" name="linkedin"></MyIcon
        ></a>
      </div>
      <div class="footer-coordoné">
        <a class="link" href="mailto:meldryck.d.said@gmail.com<">
          <MyTitle el="h5" size="small">
            <h2 class="footer__title">meldryck.d.said@gmail.com</h2>
          </MyTitle>
        </a>
        <a class="link" href="tel:+33772428966">
          <MyTitle el="h5" size="small">
            <h2 class="footer__title">+33 7 72 42 89 66</h2>
          </MyTitle>
        </a>
      </div>
    </div>
    <div class="footer-link">
      <RouterLink class="link" :to="`/Contact`"> Contact </RouterLink>
      <RouterLink class="link" :to="`/Projets`"> Projets </RouterLink>
    </div>
  </div>
</template>

<style lang="scss">
.footer__content {
  height: 263px;

  background-color: $D;
  display: flex;
  justify-content: space-around;
  align-items: center;
  margin-top: 20px;
}
.footer-link {
  display: flex;
  justify-content: space-around;
  width: 18%;
}
.link {
  color: $L;
  font-family: $secondary-font;
  font-weight: 700;
  display: inline-block;
  text-decoration: none;
  padding: 10px;
  gap: 25px;
  position: relative;
}

.link::after {
  content: "";
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translateX(50%);
  width: 0%;
  height: 4px;
  background-color: $L;
  color: $L;
  transition: width 0.3s ease-out, left 0.3s ease-out;
}

.link::before {
  content: "";
  position: absolute;
  bottom: 0;
  right: 50%;
  transform: translateX(-50%);
  width: 0%;
  height: 4px;
  background-color: $L;
  color: $D;
  transition: width 0.3s ease-out, right 0.3s ease-out;
}

.link:hover::after {
  width: 50%;
  left: 0%;
}

.link:hover::before {
  width: 50%;
  right: 0%;
}

.footer-information {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: max-content;
  .footer-social {
    display: flex;
    gap: 30px;
    align-items: center;
    justify-content: space-around;
    flex-direction: row;
  }
  .footer__title {
    text-align: center;
    color: $L;
  }
}

@media screen and (max-width: 425px) {

  
  .footer__content {
    height: auto;
    background-color: $D;
    display: flex;
    flex-direction: column-reverse;
    justify-content: space-around;
    align-items: center;
    margin-top: 20px;
  }
  .footer-link {
    display: flex;
    justify-content: center;
    flex-direction: column;
    width: 18%;
  }
  .link {
    color: $L;
    font-family: $secondary-font;
    font-weight: 700;
    text-decoration: none;
    padding: 10px;
    gap: 25px;
    position: relative;
  }

  .link::after {
    content: "";
    position: absolute;
    bottom: 0;
    left: 50%;
    transform: translateX(50%);
    width: 0%;
    height: 4px;
    background-color: $L;
    color: $L;
    transition: width 0.3s ease-out, left 0.3s ease-out;
  }

  .link::before {
    content: "";
    position: absolute;
    bottom: 0;
    right: 50%;
    transform: translateX(-50%);
    width: 0%;
    height: 4px;
    background-color: $L;
    color: $D;
    transition: width 0.3s ease-out, right 0.3s ease-out;
  }

  .link:hover::after {
    width: 50%;
    left: 0%;
  }

  .link:hover::before {
    width: 50%;
    right: 0%;
  }

  .footer-information {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: max-content;
    .footer-social {
      display: flex;
      gap: 30px;
      align-items: center;
      justify-content: space-around;
      flex-direction: row;
      scale: 0.8;
    }
    .footer__title {
      text-align: center;
      color: $L;
    }
  }
}

@media screen and (min-width: 725px) and (max-width: 1024px) {

  
  .footer__content {
    height: auto;
    background-color: $D;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    margin-top: 20px;
  }
  .footer-link {
    display: flex;
    justify-content: center;
    flex-direction: column;
    width: 18%;
  }
  .link {
    color: $L;
    font-family: $secondary-font;
    font-weight: 700;
    text-decoration: none;
    padding: 10px;
    gap: 25px;
    position: relative;
  }

  .link::after {
    content: "";
    position: absolute;
    bottom: 0;
    left: 50%;
    transform: translateX(50%);
    width: 0%;
    height: 4px;
    background-color: $L;
    color: $L;
    transition: width 0.3s ease-out, left 0.3s ease-out;
  }

  .link::before {
    content: "";
    position: absolute;
    bottom: 0;
    right: 50%;
    transform: translateX(-50%);
    width: 0%;
    height: 4px;
    background-color: $L;
    color: $D;
    transition: width 0.3s ease-out, right 0.3s ease-out;
  }

  .link:hover::after {
    width: 50%;
    left: 0%;
  }

  .link:hover::before {
    width: 50%;
    right: 0%;
  }

  .footer-information {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: max-content;
    .footer-social {
      display: flex;
      gap: 30px;
      align-items: center;
      justify-content: space-around;
      flex-direction: row;
      scale: 0.8;
    }
    .footer__title {
      text-align: center;
      color: $L;
    }
  }
}
</style>

<script setup></script>
