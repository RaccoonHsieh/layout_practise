<template>
  <div class="jumbotron">
    <div class="banner">
      <span class="icon banner-icon-1"></span>
      <span class="icon banner-icon-2"></span>
      <span class="icon banner-icon-3"></span>
      <span class="icon banner-icon-4"></span>
      <span class="icon banner-icon-5"></span>
      <span class="icon banner-icon-6"></span>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.jumbotron {
  width: 100%;
  height: 400px;
  background-color: #ffe9f3;

  .banner {
    .icon {
      position: absolute;
      z-index: 100;
    }
    .banner-icon-1 {
      background-image: url(../../../assets/layout_practise/kv-icon-1.svg);
      background-repeat: no-repeat;
      background-size: contain;
      width: 10vw;
      height: 10vh;
      top: 0;
      left: 30%;
    }
  }
}
</style>
