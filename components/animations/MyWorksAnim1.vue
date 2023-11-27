<template>
  <div>
    <svg
      width="293"
      height="393"
      viewBox="0 0 293 393"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
      class="visu"
      ref="svgRef"
    >
      <path
        d="M292 3L71.39 39.0233C25.6067 46.4993 22.4771 111.168 67.3246 123.03V123.03C101.212 131.993 110.712 175.559 83.6331 197.817L32.1444 240.138C-18.021 281.371 2.1071 362.354 65.7394 375.304L135.5 389.5"
        stroke="black"
        stroke-width="6"
      />
    </svg>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue';
import ScrollMagic from 'scrollmagic';

const svgRef = ref(null);

onMounted(() => {
  const controller = new ScrollMagic.Controller();
  const svgElement = svgRef.value;

  new ScrollMagic.Scene({
    triggerElement: svgElement,
    offset: window.innerHeight / 2,
  })
    .addTo(controller)
    .on('enter', () => {
      svgElement.classList.add('animate');
    });
});
</script>

<style lang="scss">
.visu {
  stroke-dasharray: 600;
  stroke-dashoffset: 1000;
  &.animate {
    animation: dash 1s linear forwards;
  }
}

@keyframes dash {
  from {
    stroke-dashoffset: 1000;
  }
  to {
    stroke-dashoffset: 0;
  }
}
</style>
