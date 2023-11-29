<template>
  <svg
    class="waves"
    width="500"
    height="139"
    viewBox="0 0 500 139"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      d="M3.49991 1C-11.0002 211 442.499 68 497.5 137"
      stroke="black"
      stroke-width="6"
    ></path>
  </svg>
</template>
<script setup></script>
<style lang="scss">
.waves {
  stroke-dasharray: 600;
  stroke-dashoffset: 100;
  animation: dash 5s linear forwards;
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
