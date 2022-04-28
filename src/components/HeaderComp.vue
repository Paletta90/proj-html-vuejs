<template>

    <div id="header">

        <!-- NavBar sinistra-->
        <NavbarComp />

        <!-- Logo centrale -->
        <LogoComp />

        <!-- Sezione input -->
        <InputComp />

    </div>

</template>

<script>
    // Import components
    import NavbarComp from './partial/NavbarComp.vue'
    import LogoComp from './partial/LogoComp.vue'
    import InputComp from './partial/InputComp.vue'

    export default {
        name: 'HeaderComp',

        // Componenti
        components: {
            NavbarComp,
            LogoComp,
            InputComp
        }

    }

</script>

<style lang="scss" scoped>
    // Import file.scss
    @import '../style/mixin.scss';

    #header{
        // Centro al x%
        @include center-x(90%);
        // Flex orizzonatalmente header
        @include flex(row, space-between, center);

        padding: 20px 0;

        div{
            width: calc(100% / 3);
            // @include flex(row, space-between, center);
        }

    }
</style>