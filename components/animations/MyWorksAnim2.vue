<template>
  <div>
    <svg
      class="visu2"
      width="144"
      height="348"
      viewBox="100 0 144 747"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
      :class="{ reversed: isReversed }"
    >
      <path
        d="M3 2L121.376 145.629C156.099 187.761 141.016 251.408 91.0936 273.51V273.51C33.7423 298.902 24.5945 376.509 74.5 414.5V414.5V414.5C138.822 467.178 148.894 561.757 97.1089 626.799L3 745"
        stroke="black"
        stroke-width="12"
      />
    </svg>
  </div>
</template>

<script setup>
defineProps({
  isReversed: Boolean,
});
</script>

<style lang="scss">
.visu2 {
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
</style>
