<template>
  <div class="app">
    <div>
      <no-ssr>
        <!--        https://github.com/apertureless/vue-parallax/issues/10-->
        <div style="position: relative; z-index: 9999; background-color: #fff;">
          <h1 style="margin:0;">Meadows Wedding</h1>
          <h2 style="margin:0;">19<small>th</small> March 2022</h2>
          <parallax :speedFactor="speedFactorSpeed">
            <img src="/brighton.jpg" alt="very cool bg">
          </parallax>
        </div>

        <div style="background-color: #fff; height: 50vh;">
          <h1>Blank body</h1>
        </div>

        <div style="position: relative;">
          <parallax :speedFactor="speedFactorSpeed" :fixed="true">
            <img src="/engadgement.jpg" alt="very cool bg">
          </parallax>
        </div>
        
        <div style="position: relative; z-index: 9999; background-color: #fff;">
          <parallax :speedFactor="speedFactorSpeed">
            <img src="/leggies.jpg" alt="very cool bg">
          </parallax>
        </div>
        
        
        <div style="background-color: #fff; height: 50vh;">
          <h1>Blank body</h1>
        </div>

        <div style="position: relative;">
          <parallax :speedFactor="speedFactorSpeed" :fixed="false">
            <img src="/prague.jpg" alt="very cool bg">
          </parallax>
        </div>

        <div style="position: relative;">
          <parallax :speedFactor="speedFactorSpeed">
            <img src="/poser.jpg" alt="very cool bg">
          </parallax>
        </div>
        <!--      <parallax :speedFactor="{speedFactor}">-->
        <!--        <img src="/ballet.jpg" alt="very cool bg">-->
        <!--      </parallax>-->

        <!--      <parallax :speedFactor="{speedFactor}">-->
        <!--        <img src="/kitty.jpg" alt="very cool bg">-->
        <!--      </parallax>-->
      </no-ssr>

    </div>
    test

  </div>
</template>

<script>
  import Parallax from 'vue-parallaxy'

  export default {
    components: {
      Parallax
    },
    data: function () {
      return {
        speedFactorSpeed: 0.01
      }
    },
  }
</script>

<style>
  body {
    margin: 0;
  }

  .app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    position: relative;
  }
</style>
