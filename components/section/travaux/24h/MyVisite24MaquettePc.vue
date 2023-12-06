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
        "https://www.figma.com/proto/rTbZa7tR7zD20RaUZmo60j/Projet-co-S3_D%C3%A9fi_24h?page-id=1101%3A818&type=design&node-id=2609-834&viewport=513%2C147%2C0.03&t=IbTQgM61Ety8Y9os-1&scaling=scale-down&starting-point-node-id=3082%3A933&mode=design";

      window.open(url, "_blank");
    },
  },
};
</script>
