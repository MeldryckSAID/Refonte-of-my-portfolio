<!-- <template>
  <div class="app">
    <div class="header" :class="{ 'header--fixed': isHeaderFixed }">
      <header class="layout__header">
        <MyHeader />
      </header>
    </div>
    <div class="main-content">
      <NuxtPage />
    </div>
    <footer>
      <MyFooter />
    </footer>
  </div>
</template>

<style lang="scss" scoped>
.app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;

}

.header {
  width: 100%;
  position: fixed;
  top: 0;
  background-color: $L;
  z-index: 1000;
  transition: background-color 0.3s; 
}

.header--fixed {
  background-color: $L; 
}

.main-content {
  flex: 1;
  margin-top: 10%; 
}

footer {
  margin-top: auto; 
}
</style>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";

const isHeaderFixed = ref(false);

const handleScroll = () => {
  isHeaderFixed.value = window.scrollY > 0;
};

onMounted(() => {
  window.addEventListener("scroll", handleScroll);
});

onUnmounted(() => {
  window.removeEventListener("scroll", handleScroll);
});
</script> -->

<template>
  <div class="app">
    <div v-if="isUnderMaintenance">
      <MyHeader />
      <MyMaintenance />
      <MyFooter />
    </div>
    <div v-else>
      <div class="header" :class="{ 'header--fixed': isHeaderFixed }">
        <header class="layout__header">
          <MyHeader />
        </header>
      </div>
      <div class="main-content">
        <NuxtPage />
      </div>
      <footer v-show="!isUnderMaintenance">
        <MyFooter />
      </footer>
    </div>
  </div>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";

const isUnderMaintenance = ref(false);
const isHeaderFixed = ref(false);

const handleScroll = () => {
  isHeaderFixed.value = window.scrollY > 0;
};

const checkMaintenance = () => {
  const isMobile = window.matchMedia("(max-width: 1024px)").matches;
  isUnderMaintenance.value = isMobile;
};

onMounted(() => {
  console.log("Mounted. Checking maintenance...");
  checkMaintenance();
  window.addEventListener("resize", checkMaintenance);
  window.addEventListener("scroll", handleScroll);
});

onUnmounted(() => {
  window.removeEventListener("resize", checkMaintenance);
  window.removeEventListener("scroll", handleScroll);
});
</script>

<style lang="scss" scoped>
.app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.header {
  width: 100%;
  position: fixed;
  top: 0;
  background-color: $L;
  z-index: 1000;
  transition: background-color 0.3s;
}

.header--fixed {
  background-color: $L;
}

.main-content {
  flex: 1;
  margin-top: 10%;
}

footer {
  margin-top: auto;
}
</style>
