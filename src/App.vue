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

  </div>

</template>

<script>
  // Import components
  import HeaderComp from './components/HeaderComp.vue'
  import MainComp from './components/MainComp.vue'

  export default {

    name: 'App',

    components: {
      HeaderComp,
      MainComp
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

    // Utility
    .circle {
      width: 55px;
      height: 55px;
      border-radius: 50%;
      border: 7px solid $color-texasRose;
    }

  }
</style>