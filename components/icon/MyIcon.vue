<script setup>
import { computed } from "vue";
import Git from "../components/icon/Git.vue";
import Linkedin from "../components/icon/Linkedin.vue";
import Git__black from "../components/icon/Git__black.vue";
import Linkedin__black from "../components/icon/Linkedin__black.vue";

const props = defineProps({
  name: String,
  color: String,
  stroke: String,
  size: String,
  fill: String,
});
const getIcon = computed(() => {
  switch (props.name) {
    case "git":
      return Git;
    case "linkedin":
      return Linkedin;
    case "gitn":
      return Git__black;
    case "linkedinn":
      return Linkedin__black;

    default:
      return Linkedin;
  }
});

const className = computed(() => ({

  " -primary": props.color === "primary",
  " -secondary": props.color === "secondary",

 
  " -sprimary": props.stroke === "primary",
  " -ssecondary": props.stroke === "secondary",
  " -ssans": props.stroke === "base",

  " -small": props.size === "small",
  " -regular": props.size === "regular",
  " -big": props.size === "big",

 
  " -fblack": props.fill === "black",
  " -fsans": props.fill === "base",
  " -fwhite": props.fill === "white",
}));
</script>

<template>
  <i :class="className" class="icon">
    <component :is="getIcon" />
  </i>
</template>

<style lang="scss" scoped>
.icon {
  align-items: center;
  border-radius: 100%;
  box-shadow: 0 0 rem(5) 0 $L;
  display: inline-flex;
  height: rem(50);
  justify-content: center;
  width: rem(50);

  //background
  &.-primary {
    background: $D;
  }
  &.-secondary {
    background: $L;
  }

  //fill
  &-.fwhite {
    fill: $L;
  }
  &-.fblack {
    fill: $D;
  }
  &-.fsans {
    fill: none;
  }

  //stroke

  &.-sprimary {
    color: $D;
  }
  &.-ssecondary {
    color: $L;
  }

  &.-ssans {
    color: none;
  }
  //Size
  &.-small {
    svg {
      scale: 0.5;
    }
    height: rem(25);
    width: rem(25);
  }
  &.-regular {
    height: rem(50);
    width: rem(50);
  }
  &.-big {
    svg {
      scale: 1.5;
    }
    height: rem(100);
    width: rem(100);
  }
}
</style>
