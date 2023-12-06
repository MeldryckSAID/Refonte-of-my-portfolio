<template>
  <div>
    <Mybutton @click="ouvrirMiniFenetre()"><slot></slot></Mybutton>
  </div>
</template>

<script>
export default {
  methods: {
    ouvrirMiniFenetre() {
      // L'URL du site que vous souhaitez ouvrir
      const url =
        "https://www.figma.com/proto/b9J9XFfjSPUWNwz9Tua18b/Projet-Co-%7C-Expo-Artistique?page-id=266%3A787&type=design&node-id=266-942&viewport=1148%2C535%2C0.19&t=vA8OW7BP63VlJucH-1&scaling=min-zoom&starting-point-node-id=266%3A942&mode=design";

      window.open(url, "_blank");
    },
  },
};
</script>
