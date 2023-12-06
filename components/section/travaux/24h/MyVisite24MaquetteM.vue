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
      const url =
        "https://www.figma.com/proto/rTbZa7tR7zD20RaUZmo60j/Projet-co-S3_D%C3%A9fi_24h?page-id=1502%3A8303&type=design&node-id=1502-8532&viewport=340%2C805%2C0.07&t=oqBeTINCLbo2v7ly-1&scaling=scale-down&starting-point-node-id=1502%3A8532&show-proto-sidebar=1&mode=design";

      window.open(url, "_blank");
    },
  },
};
</script>
