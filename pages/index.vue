<template>
  <MyIntro />

  <MyPresentation />

  <MyWorks />
  <RouterLink class="link" :to="`/Contact`"> <MyContact /> </RouterLink>

</template>
<style lang="scss"></style>
<script setup>
const { client } = usePrismic();
const { data: home } = await useAsyncData("home", () =>
  client.getSingle("Card")
);
</script>
