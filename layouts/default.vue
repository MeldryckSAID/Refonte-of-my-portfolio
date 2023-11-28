<template>
  <main class="layout">
    <div class="header" :class="{ 'header--fixed': isHeaderFixed }">
      <header class="layout__header">
        <MyHeader />
      </header>
    </div>
    <div class="cache"></div>
    <NuxtPage class="main-content" />
    <footer>
      <MyFooter />
    </footer>
  </main>
</template>
<style lang="scss" scoped>
.layout {
  display: flex;
  flex-direction: column;
}

.cache {
  width: 30px;
  height: 132px;
}
.main-content {
  margin-top: 10%;
}
.header {
  width: 100%;
  position: fixed;
  padding-top: 10px;
  top: 0;
  background-color: $L;
  z-index: 1000;
}

.header--fixed {
  position: fixed;
  background-color: $L;
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
</script>
