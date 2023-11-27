<template>
  <div :class="className"><MyLogo /></div>
</template>
<style lang="scss">
.size {
  width: 100%;

  &.--s {
    width: 50px;
  }

  &.--m {
    width: 100px;
  }

  &.--l {
    width: 350px;
  }
}
</style>
<script setup>
const className = computed(() => ({
  "--s": size.value === "small",
  "--m": size.value === "medium",
  "--l": size.value === "large",
}));
</script>
