<template>
  <div>
    <Mybutton class="btn-page" @click="ouvrirMiniFenetre()">Git du Projet</Mybutton>
  </div>
</template>

<script>
export default {
  methods: {
    ouvrirMiniFenetre() {
      // L'URL du site que vous souhaitez ouvrir
      const url = "https://github.com/MeldryckSAID/Defi_24h";

       window.open(url, "_blank");
    },
  },
};
</script>
<style lang="scss">
.btn-page{
  cursor: pointer;
}
</style>
