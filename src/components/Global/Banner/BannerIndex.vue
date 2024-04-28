<template>
  <div class="jumbotron">
    <div class="banner">
      <div class="banner-icon">
        <span class="icon banner-icon-1"></span>
        <span class="icon banner-icon-2"></span>
        <span class="icon banner-icon-3"></span>
        <span class="icon banner-icon-4"></span>
        <span class="icon banner-icon-5"></span>
        <span class="icon banner-icon-6"></span>
      </div>
      <div class="banner-title">
        <span class="icon title-color"></span>
        <span class="icon title-black"></span>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
@import '../../../assets/scss/main.scss';

.jumbotron {
  width: 100%;
  height: 400px;
  background-color: #ffe9f3;

  .banner {
    @include wrapper{
      .icon {
        position: absolute;
        z-index: 100;
      }
      .banner-icon{
        .banner-icon-1 {
        background-image: url(../../../assets/layout_practise/kv-icon-1.svg);
        background-repeat: no-repeat;
        background-size: contain;
        width: 10vw;
        height: 10vh;
        top: 0;
        left: 25%;
      }
      .banner-icon-2 {
        background-image: url(../../../assets/layout_practise/kv-icon-2.svg);
        background-repeat: no-repeat;
        background-size: contain;
        width: 10vw;
        height: 10vh;
        top: 20%;
        left: 20%;
      }
      .banner-icon-3 {
        background-image: url(../../../assets/layout_practise/kv-icon-3.svg);
        background-repeat: no-repeat;
        background-size: contain;
        width: 10vw;
        height: 10vh;
        top: 40%;
        left: 10%;
      }
      .banner-icon-4 {
        background-image: url(../../../assets/layout_practise/kv-icon-4.svg);
        background-repeat: no-repeat;
        background-size: contain;
        width: 10vw;
        height: 10vh;
        top: -5%;
        right: 30%;
      }
      .banner-icon-5 {
        background-image: url(../../../assets/layout_practise/kv-icon-5.svg);
        background-repeat: no-repeat;
        background-size: contain;
        width: 10vw;
        height: 10vh;
        top: 20%;
        right: 30%;
      }
      .banner-icon-6 {
        background-image: url(../../../assets/layout_practise/kv-icon-6.svg);
        background-repeat: no-repeat;
        background-size: contain;
        width: 10vw;
        height: 10vh;
        top: 40%;
        right: 20%;
      }
      }
      .banner-title{
        .title-color{
          background-image: url(../../../assets/layout_practise/kv-title.svg);
          background-repeat: no-repeat;
          background-size: contain;
          top: 25%;
          left: 40%;
          transform: translate(-50%, -50%);
          width: 40vw;
          height: 40vh;
          z-index: 499;
          animation-name: turn;
          animation-duration: .3s;
          animation-iteration-count: infinite;
          animation-direction: alternate;
        }
        @keyframes turn {
          from {height: 40vh;}
          to   {height: 40.5vh;}
        }
        .title-black{
          background-image: url(../../../assets/layout_practise/kv-title-black.svg);
          background-repeat: no-repeat;
          background-size: contain;
          top: 25%;
          left: 40%;
          transform: translate(-50%, -50%);
          width: 40vw;
          height: 40vh;
        }
      }
    }
  }
}
</style>
