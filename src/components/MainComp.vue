<template>

    <div>

        <!-- Section Jumbotron -->
        <JumbotronComp />

        <!-- Contenitore selle sezione centrate al x% -->
        <div id="container">

            <FirstSection />

        </div>

    </div>


</template>

<script>
    // Import components
    import JumbotronComp from './partial/JumbotronComp.vue'
    import FirstSection from './partial/section1/FirstSection.vue'

    export default {
        name: 'MainComp',

        components: {
            JumbotronComp,
            FirstSection
        }
    }
</script>

<style lang="scss" scoped>
    // Import file.scss
    @import '../style/mixin.scss';

    #container{
        @include center-x(60%)
    }
</style>