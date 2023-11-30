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
      const url = "https://www.behance.net/gallery/160735099/Ilkay_MEN-Meldryck_SAID";

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
