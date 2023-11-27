<template>
  <div class="logo" :class="className" @click="toggleTheme">
    <svg
      v-if="isBlack"
      id="Calque_2_black"
      data-name="Calque 2"
      xmlns="http://www.w3.org/2000/svg"
      viewBox="0 0 393.17 393.17"
      :class="className"
    >
      <g id="Log_fnoir">
        <circle id="cercle" cx="196.58" cy="196.58" r="196.58" />
        <polyline
          id="M"
          class="ln"
          points="98.86 303.65 98.86 89.51 196.84 195.57 294.31 95.07 292.29 301.63"
        />
        <path
          id="S"
          class="ln"
          d="m292.04,210.02l-97.73-97.73c-21.9,21.9-21.9,57.4,0,79.29h0c21.9,21.9,21.9,57.4,0,79.29l-93.18-93.18"
        />
      </g>
    </svg>

    <svg
      v-else
      id="Calque_2_white"
      data-name="Calque 2"
      xmlns="http://www.w3.org/2000/svg"
      viewBox="0 0 413.17 413.17"
      :class="className"
    >
      <g id="Log_fblanc">
        <circle id="cercle" class="fond" cx="206.58" cy="206.58" r="196.58" />
        <polyline
          id="M"
          class="trait"
          points="109 313.65 109 99.51 206.84 205.57 304.17 105.07 302.15 311.63"
        />
        <path
          id="S"
          class="trait"
          d="m301.04,220.02l-97.73-97.73c-21.9,21.9-21.9,57.4,0,79.29h0c21.9,21.9,21.9,57.4,0,79.29l-93.18-93.18"
        />
      </g>
    </svg>
  </div>
</template>

<script setup>
import { ref, onMounted, computed } from "vue";

const isBlack = ref(true);
const isWhite = ref(false);


const toggleTheme = () => {
  isBlack.value = !isBlack.value;
  isWhite.value = !isWhite.value;
};

const className = computed(() => ({
  " -small": props.size === "small",
  " -regular": props.size === "regular",
  " -big": props.size === "big",
}));
const props = defineProps({
  size: String,
});
</script>

<style lang="scss">
.logo {
  width: 100%;

  &.-small {
    svg {
      width: 98px;
    }
  }
  &.-regular {
    svg {
      width: 135px;
    }
  }
  &.-big {
    svg {
      width: 269px;
    }
  }
}
.ln {
  fill: none;
  stroke: #fff;
  stroke-miterlimit: 10;
  stroke-width: 20px;
}

.fond {
  fill: #fff;
}

.fond,
.trait {
  stroke: #000;
  stroke-miterlimit: 10;
  stroke-width: 20px;
}

.trait {
  fill: none;
}

.--white {
  fill: #fff;
}
</style>
