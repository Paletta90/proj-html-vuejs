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