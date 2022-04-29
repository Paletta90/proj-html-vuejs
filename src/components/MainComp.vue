<template>

    <div>

        <!-- Section Jumbotron -->
        <JumbotronComp />

        <!-- Contenitore selle sezione centrate al x% -->
        <div id="container">

            <!-- Prima sezione -->
            <FirstSection />

            <!-- Seconda sezione -->
            <SecondSection />

            <!-- Terza sezione -->
            <ThirdSection />

        </div>

    </div>


</template>

<script>
    // Import components
    import JumbotronComp from './partial/JumbotronComp.vue'
    import FirstSection from './partial/section1/FirstSection.vue'
    import SecondSection from './partial/section2/SecondSection.vue'
    import ThirdSection from './partial/section3/ThirdSection.vue'

    export default {
        name: 'MainComp',

        components: {
            JumbotronComp,
            FirstSection,
            SecondSection,
            ThirdSection
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