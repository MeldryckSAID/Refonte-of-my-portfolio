<template>
  <div>
    <Mybutton class="btn-page" @click="ouvrirMiniFenetre()"><slot></slot></Mybutton>
  </div>
</template>

<script>
export default {
  methods: {
    ouvrirMiniFenetre() {
      // L'URL du site que vous souhaitez ouvrir
      const url = "https://transcendent-kulfi-b28e20.netlify.app/";

       window.open(url, "_blank");
    },
  },
};
</script>
