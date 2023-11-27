<template>
  <div>
    <svg
      width="293"
      height="393"
      viewBox="0 0 1 393"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
      class="visu"
      ref="svgRef"
    >
      <path
        d="M292 3L71.39 39.0233C25.6067 46.4993 22.4771 111.168 67.3246 123.03V123.03C101.212 131.993 110.712 175.559 83.6331 197.817L32.1444 240.138C-18.021 281.371 2.1071 362.354 65.7394 375.304L135.5 389.5"
        stroke="black"
        stroke-width="6"
        :style="{ strokeDasharray: state.strokeDashArray, strokeDashoffset: state.strokeDashOffset }"
      />
    </svg>
  </div>
</template>

<script setup>
import { ref, onMounted, onBeforeUnmount, reactive } from 'vue';

const svgRef = ref(null);
const state = reactive({
  strokeDashArray: 200,
  strokeDashOffset: 50, // Commence à la fin de la ligne
  scrollSpeed: 0.1, // Coefficient pour ajuster la vitesse
});

const updateDashOffset = () => {
  const svgElement = svgRef.value;
  const rect = svgElement.getBoundingClientRect();
  const triggerPoint = rect.top + window.innerHeight * 0.5;

  if (window.scrollY > triggerPoint) {
    state.strokeDashOffset = state.strokeDashArray - (window.scrollY - triggerPoint) * state.scrollSpeed;
    if (state.strokeDashOffset < 0) {
      state.strokeDashOffset = 0;
    }
  }
};

onMounted(() => {
  updateDashOffset(); // Mise à jour initiale

  window.addEventListener('scroll', updateDashOffset);
});

// Assurez-vous de nettoyer les écouteurs d'événements lorsque le composant est démonté
onBeforeUnmount(() => {
  window.removeEventListener('scroll', updateDashOffset);
});
</script>

<style lang="scss">
/* Ajoutez vos styles ici */
</style>
