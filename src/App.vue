<template>

  <div id="app">

    <!-- Header -->
    <header>

      <!-- Componente che contiene header -->
      <HeaderComp />

    </header>

    <!-- Main -->
    <main>

      <MainComp />

    </main>

    <!-- Footer -->
    <footer>

      <FooterComp />

    </footer>

  </div>

</template>

<script>
  // Import components
  import HeaderComp from './components/HeaderComp.vue'
  import MainComp from './components/MainComp.vue'
  import FooterComp from './components/FooterComp.vue'

  export default {

    name: 'App',

    components: {
      HeaderComp,
      MainComp,
      FooterComp
    }

  }
</script>

<style lang="scss">
  // Import file.scss
  @import './style/mixin.scss';
  @import './style/variabili.scss';

  // Mixin per reset
  * {
    @include reset()
  }

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;

    footer{
      background-color: $color-vulcan;
    }
    // Utility
    .circle {
      width: 55px;
      height: 55px;
      border-radius: 50%;
      border: 7px solid $color-texasRose;
    }

    .small-title {
      @include font(initial, 500, $color-gunSmoke);
      text-transform: uppercase;
      margin-bottom: 15px;
    }

    .paragraph {
      @include font($font-sizeNavbar, 500, $color-gunSmoke);
      line-height: 20px;
    }

    .textColor{
      @include font($font-titleh2, 100, $color-mountainMeadow);
    }
    .textBold{
      @include font($font-sizeNavbar, 1000, $color-stormDust);
    }
    .text-center{
      text-align: center;
    }

  }
</style>