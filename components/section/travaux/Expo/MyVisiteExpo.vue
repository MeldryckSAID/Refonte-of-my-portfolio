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
        "https://www.figma.com/proto/b9J9XFfjSPUWNwz9Tua18b/Projet-Co-%7C-Expo-Artistique?page-id=0%3A1&type=design&node-id=87-267&viewport=-2632%2C-373%2C0.25&t=nAV17loCt6Zy3pno-1&scaling=min-zoom&starting-point-node-id=87%3A267&mode=design";

      const largeur = Math.round(window.innerWidth * 0.85);
      const hauteur = Math.round(window.innerHeight * 0.85);

      const options = `width=${largeur},height=${hauteur},left=${
        (window.innerWidth - largeur) / 2
      },top=${(window.innerHeight - hauteur) / 2}`;

      window.open(url, "_blank", options);
    },
  },
};
</script>
