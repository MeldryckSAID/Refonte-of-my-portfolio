<template>
  <nuxt-link
    :to="to"
    v-if="to"
    class="button tcolor"
    @mouseover="hoverEffect(true)"
    @mouseout="hoverEffect(false)"
    :class="className"
  >
    <slot></slot>
  </nuxt-link>
  <button
    v-else
    class="button tcolor"
    :class="className"
    @mouseover="hoverEffect(true)"
    @mouseout="hoverEffect(false)"
  >
    <slot></slot>
  </button>
</template>

<style lang="scss" scoped>
.button {
  position: relative;
  border: 2px solid $D;
  border-radius: rem(15);
  display: inline-block;
  font-family: $secondary-font;
  font-size: 15px;
  font-weight: 600;
  text-decoration: none;
  word-wrap: break-word;
  width: 178px;
  height: 52px;
  flex-shrink: 0;
  overflow: hidden;
  background: linear-gradient(to left, $D 50%, $L 50%);
  background-size: 200% 100%;
  transition: background-position 0.3s, color 0.3s;
}

.button:hover {
  background-position: 100% 0;
  color: $L;
  box-shadow: inset 0 0 0 2px rgba($D, 0.5), 0 0 0;
}

.button.-ssecondary {
  background: linear-gradient(to left, $D 50%, $L 50%);
}
</style>

<script setup>
const props = defineProps({
  to: String,
});

const hoverEffect = (isHovered) => {
  const button = document.querySelector(".button");
  if (button) {
    button.style.backgroundPosition = isHovered ? "100% 0" : "0% 0";
  }
};
</script>
