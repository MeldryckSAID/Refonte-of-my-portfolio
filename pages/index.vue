<template>
  <MyIntro />

  <MyPresentation />

  <MyCard
    id="1"
    paragraphe="Le défi 24 heures était un défie plein d'émotion incroyable et intrépide 
    Pourrez-vous comprendre toute ça complicité  Le défi 24 heures est événement phares du département MMI Montbéliard ..."
    image="/png/24h.png"
  />
</template>
<style lang="scss"></style>
<script setup>
const { client } = usePrismic();
const { data: home } = await useAsyncData("home", () =>
  client.getSingle("Card")
);
</script>
