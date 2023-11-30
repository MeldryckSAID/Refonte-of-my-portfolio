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
        "hhttps://www.figma.com/proto/lgyjbhSTzCjmhzH7YTesrh/Phase-design-concept?page-id=0%3A1&type=design&node-id=1-2&viewport=207%2C409%2C0.04&t=chGqxVlpHMfPq0xE-1&scaling=scale-down&starting-point-node-id=1%3A2&show-proto-sidebar=1&mode=design";

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
