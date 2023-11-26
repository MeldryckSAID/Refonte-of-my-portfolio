<template>
  <div class="header__content">
    <RouterLink :to="`/`">
      <MyLogo class="Logo_header" />
    </RouterLink>
    <div class="header-link">
      <RouterLink class="link_router" :to="`/Contact`"> Contact </RouterLink>
      <RouterLink class="link_router" :to="`/Projets`"> Projets </RouterLink>
    </div>
  </div>
</template>

<style lang="scss">
.header__content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom:20px;
  border-bottom: 2px solid $D
}
.header-link {
  display: flex;
  justify-content: space-between;
}

.Logo_header {
  width: 97.47px;
}

.link_router {
  text-decoration: none;
  color: $D;
  font-family: $secondary-font;
  font-weight: 700;
  display: inline-block;
  margin: 0;
  padding: 10px;
  gap: 25px;
  position: relative;
}

.link_router::after {
  content: "";
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translateX(50%);
  width: 0%;
  height: 4px;
  background-color: $D;
  color: $D;
  transition: width 0.3s ease-out, left 0.3s ease-out;
}

.link_router::before {
  content: "";
  position: absolute;
  bottom: 0;
  right: 50%;
  transform: translateX(-50%);
  width: 0%;
  height: 4px;
  background-color: $D;
  color: $D;
  transition: width 0.3s ease-out, right 0.3s ease-out;
}

.link_router:hover::after {
  width: 50%;
  left: 0%;
}

.link_router:hover::before {
  width: 50%;
  right: 0%;
}
</style>

<script setup></script>
