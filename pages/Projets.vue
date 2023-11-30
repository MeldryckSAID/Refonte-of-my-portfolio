<template>
  <MyIntroTravaux>Mes travaux</MyIntroTravaux>
  <MyWorksComplete />
</template>
<style lang="scss">
h1 {
  font-family: $primary-font;
}
.test {
  display: flex;
  flex-direction: row;
  gap: 200px;
}
</style>
<script setup>
useSeoMeta({
  title: "SAÏD Meldryck//Projet",
  ogTitle: "SAÏD Meldryck",
  description: "L'ensemble de mes projets ",
  ogDescription: "L'ensemble de mes projets ",
  ogImage: "/favicon.png",
});
</script>
