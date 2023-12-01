<script setup>
import { computed } from "vue";
import figma from "../components/tech/figma.vue";
import adobe_aftereffects from "../components/tech/adobe_aftereffects.vue";
import adobe_illustrator from "../components/tech/adobe_illustrator.vue";
import adobe_photoshop from "../components/tech/adobe_photoshop.vue";
import adobe_premiere from "../components/tech/adobe_premiere.vue";
import Davinci from "../components/tech/DaVinci.vue";
import css3 from "../components/tech/css3.vue";
import html from "../components/tech/html.vue";
import indesign from "../components/tech/indesign.vue";
import JS from "../components/tech/JS.vue";
import nodejs from "../components/tech/nodejs.vue";
import Nuxtjs from "../components/tech/Nuxtjs.vue";
import vuejs from "../components/tech/vuejs.vue";
import wordpress from "../components/tech/wordpress.vue";
import firebase from "../components/tech/firebase.vue";
import supabase from "../components/tech/supabase.vue";
import tailwind from "../components/tech/tailwind.vue";
import threejs from "../components/tech/threejs.vue";
import unreal from "../components/tech/unreal.vue";
import vercel from "../components/tech/vercel.vue";
import blender from "../components/tech/blender.vue";
import dddsmax from "../components/tech/dddsmax.vue";

const props = defineProps({
  name: String,
  size: String,
});
const getTech = computed(() => {
  switch (props.name) {
    case "figma":
      return figma;
    case "ae":
      return adobe_aftereffects;
    case "pr":
      return adobe_premiere;
    case "ai":
      return adobe_illustrator;
    case "ap":
      return adobe_photoshop;
    case "css":
      return css3;
    case "html":
      return html;
    case "indi":
      return indesign;
    case "js":
      return JS;
    case "node":
      return nodejs;
    case "nuxt":
      return Nuxtjs;
    case "vue":
      return vuejs;
    case "wp":
      return wordpress;
    case "firebase":
      return firebase;
    case "supa":
      return supabase;
    case "tail":
      return tailwind;
    case "unreal":
      return unreal;
    case "max":
      return dddsmax;
    case "three":
      return threejs;
    case "vercel":
      return vercel;
    case "blender":
      return blender;
    case "davinci":
      return Davinci;

    default:
      return figma;
  }
});

const className = computed(() => ({
  " -small": props.size === "small",
  " -regular": props.size === "regular",
  " -big": props.size === "big",

  " -fblack": props.fill === "black",
  " -fsans": props.fill === "base",
  " -fwhite": props.fill === "white",
}));
</script>

<template>
  <i :class="className" class="tech">
    <component :is="getTech" />
  </i>
</template>

<style lang="scss" scoped>
.tech {
  align-items: center;
  border-radius: 100%;
  box-shadow: 0 0 rem(5) 0 $L;
  display: inline-flex;
  height: rem(50);
  justify-content: center;
  width: rem(50);

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
