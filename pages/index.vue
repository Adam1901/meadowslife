<template>
  <div class="">
    <div>
      <no-ssr>
<!--        https://github.com/apertureless/vue-parallax/issues/10-->
        <parallax :speedFactor="speedFactorSpeed">
          <img src="/brighton.jpg" alt="very cool bg">
        </parallax>

        <div style="position: relative;">
          <parallax :speedFactor="speedFactorSpeed" :fixed="false">
            <img src="/engadgement.jpg" alt="very cool bg">
          </parallax>
        </div>
        <parallax :speedFactor="speedFactorSpeed">
          <img src="/leggies.jpg" alt="very cool bg">
        </parallax>

        <parallax :speedFactor="speedFactorSpeed">
          <img src="/prague.jpg" alt="very cool bg">
        </parallax>

        <parallax :speedFactor="speedFactorSpeed">
          <img src="/poser.jpg" alt="very cool bg">
        </parallax>

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
  .container {
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
  }

  .title {
    font-family: 'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
    display: block;
    font-weight: 300;
    font-size: 100px;
    color: #35495e;
    letter-spacing: 1px;
  }

  .subtitle {
    font-weight: 300;
    font-size: 42px;
    color: #526488;
    word-spacing: 5px;
    padding-bottom: 15px;
  }

  .links {
    padding-top: 15px;
  }
</style>
