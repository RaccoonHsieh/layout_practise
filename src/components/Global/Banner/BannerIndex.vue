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
      <div class="people man"></div>
      <div class="people woman"></div>
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
    height: 100%;
    overflow: hidden;
    @include wrapper{
      .icon {
        position: absolute;
        z-index: 3;
      }
      .banner-icon{
        .banner-icon-1 {
        background-image: url(../../../assets/layout_practise/kv-icon-1.svg);
        background-repeat: no-repeat;
        background-size: contain;
        width: 5vw;
        height: 5vw;
        top: 40%;
        left: 4%;
      }
      .banner-icon-2 {
        background-image: url(../../../assets/layout_practise/kv-icon-2.svg);
        background-repeat: no-repeat;
        background-size: contain;
        width: 7vw;
        height: 7vw;
        top: 15%;
        left: 10%;
      }
      .banner-icon-3 {
        background-image: url(../../../assets/layout_practise/kv-icon-3.svg);
        background-repeat: no-repeat;
        background-size: contain;
        width: 5vw;
        height: 5vw;
        top: 0%;
        left: 20%;
      }
      .banner-icon-4 {
        background-image: url(../../../assets/layout_practise/kv-icon-4.svg);
        background-repeat: no-repeat;
        background-size: contain;
        width: 5vw;
        height: 5vw;
        top: 20%;
        right: 10%;
      }
      .banner-icon-5 {
        background-image: url(../../../assets/layout_practise/kv-icon-5.svg);
        background-repeat: no-repeat;
        background-size: contain;
        width: 8vw;
        height: 8vw;
        top: -3%;
        right: 15%;
      }
      .banner-icon-6 {
        background-image: url(../../../assets/layout_practise/kv-icon-6.svg);
        background-repeat: no-repeat;
        background-size: contain;
        width: 7vw;
        height: 7vw;
        top: 40%;
        right: 5%;
      }
      }
      .banner-title{
        height: 100%;
        .title-color{
          background-image: url(../../../assets/layout_practise/kv-title.svg);
          background-repeat: no-repeat;
          background-size: contain;
          top: 25%;
          left: 50%;
          transform: translate(-50%, -50%);
          width: 40vw;
          height: 40vh;
          z-index: 499;
          animation-name: turn;
          animation-duration: .5s;
          animation-iteration-count: infinite;
          animation-direction: alternate;
        }
        @keyframes turn {
          from {height: 40vh;}
          to   {height: 41vh;}
        }
        .title-black{
          background-image: url(../../../assets/layout_practise/kv-title-black.svg);
          background-repeat: no-repeat;
          background-size: contain;
          top: 25%;
          left: 50%;
          transform: translate(-50%, -50%);
          width: 40vw;
          height: 40vh;
        }
      }
    }
  }

  .people{
    position: absolute;
    overflow: hidden;
  }
  .man{
    background-image: url(../../../assets/layout_practise/kv-man.svg);
    background-repeat: no-repeat;
    background-size: contain;
    width: 15vw;
    height: 20vw;
    top: 16%;
    left: 17%;
  }
  .woman{
    background-image: url(../../../assets/layout_practise/kv-woman.svg);
    background-repeat: no-repeat;
    background-size: contain;
    width: 13vw;
    height: 20vw;
    top: 16%;
    right: 17%;
  }
}
</style>
