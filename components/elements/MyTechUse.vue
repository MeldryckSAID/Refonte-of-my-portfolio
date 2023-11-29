<template>
  <div class="container">
    <p>Hello c'est un test</p>
    <div class="container-child">
      <p>Hello c'est le test réussi</p>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.container {
  background-color: red;
  width: 300px;
  height: 100px;
  position: relative;

  &-child {
    width: 300px;
    height: 100px;
    background-color: green;
    position: absolute;
    top: 0;
    display: none;
  }
}

.container:hover {
  background-color: green;
}
</style>
<script setup></script>
