<template>

  <div id="app">

    <!-- Header -->
    <header>

      <!-- Componente che contiene header -->
      <HeaderComp />

    </header>

  </div>

</template>

<script>
  // Import components
  import HeaderComp from './components/HeaderComp.vue'

  export default {

    name: 'App',

    components: {
      HeaderComp
    }
  }
</script>

<style lang="scss">
  // Import file.scss
  @import './style/mixin.scss';

  // Mixin per reset
  * {
    @include reset()
  }

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }
</style>