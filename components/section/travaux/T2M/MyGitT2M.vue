<template>
  <div>
    <Mybutton class="btn-page" @click="ouvrirMiniFenetre()"
      >Git du Projet</Mybutton
    >
  </div>
</template>

<script>
export default {
  methods: {
    ouvrirMiniFenetre() {
      // L'URL du site que vous souhaitez ouvrir
      const url = "https://github.com/MeldryckSAID/Projet_Time2match";

      window.open(url, "_blank");
    },
  },
};
</script>
<style lang="scss"></style>
