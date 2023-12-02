<template>
  <div>
    <svg
      class="animchill"
      width="300"
      height="106"
      viewBox="0 0 584 106"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path
        d="M580.5 102.5L532.375 29.75C509.56 -4.73875 458.94 -4.73872 436.125 29.75V29.75C413.31 64.2387 362.69 64.2387 339.875 29.75V29.75C317.06 -4.73872 266.44 -4.73872 243.625 29.75V29.75C220.81 64.2387 170.19 64.2387 147.375 29.75V29.75C124.56 -4.73872 73.9397 -4.73875 51.125 29.75L3 102.5"
        stroke="black"
        stroke-width="6"
        stroke-linecap="round"
      />
    </svg>
  </div>
</template>

<script setup>
defineProps({
  isReversed: Boolean,
});
</script>

<style lang="scss" scoped>
.animchill {
  stroke-dasharray: 800;
  stroke-dashoffset: 100;
  animation: dash 5s linear infinite;
}
.reversed {
  transform: scaleX(-1);
}

@keyframes dash {
  from {
    stroke-dashoffset: 1000;
  }
  to {
    stroke-dashoffset: 0;
  }
}

@media screen and (max-width: 1023px) {
  svg {
    stroke-width: 20;
  }
  .animchill {
    width: 70%;
  }
}
</style>
