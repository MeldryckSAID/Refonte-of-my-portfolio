<template>
  <svg
    width="372"
    height="371"
    viewBox="0 0 572 371"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      class="sound"
      d="M0.999957 93.7617L9.18934 99.4363C72.2012 143.099 67.7975 237.646 0.999857 275.262V275.262"
      stroke="black"
      stroke-width="2"
    ></path>
    <path
      class="sound"
      d="M52.3763 54.3643V54.3643C159.197 104.418 163.347 254.82 59.4488 310.688L52.3763 314.491"
      stroke="black"
      stroke-width="4"
    ></path>
    <path
      class="sound"
      d="M119.928 3.09094V3.09094C298.364 48.9963 310.649 297.737 137.604 361.001L119.928 367.464"
      stroke="black"
      stroke-width="6"
    ></path>
  </svg>
</template>

<script setup></script>

<style lang="scss">
.sound {
  opacity: 0;
  animation: fadeIn 1s linear forwards;
}

.sound:nth-child(1) {
  animation-delay: 5s;
}

.sound:nth-child(2) {
  animation-delay: 5.5s;
}

.sound:nth-child(3) {
  animation-delay: 6s;
}

@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
</style>
