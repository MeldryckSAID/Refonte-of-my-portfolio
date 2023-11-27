<template>
  <h1>hello world its projet</h1>
  <MyLogo :iswhite="true" />
  <div class="test">
    <MyLogo size="small" />
    <MyLogo themeColor="white" size="regular" />
    <MyLogo size="regular" themeColor="white" />

    <MyLogo size="big" />
  </div>
</template>
<style lang="scss">
h1 {
  font-family: $primary-font;
}
.test {
  display: flex;
  flex-direction: row;
  gap: 200px;
}
</style>
<script setup></script>
