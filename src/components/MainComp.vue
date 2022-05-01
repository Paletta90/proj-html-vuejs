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

            <!-- Quarta sezione -->
            <FourthSection />

        </div>

    </div>


</template>

<script>
    // Import components
    import JumbotronComp from './partial/header/JumbotronComp.vue'
    import FirstSection from './partial/section1/FirstSection.vue'
    import SecondSection from './partial/section2/SecondSection.vue'
    import ThirdSection from './partial/section3/ThirdSection.vue'
    import FourthSection from './partial/section4/FourthSection.vue'

    export default {
        name: 'MainComp',

        components: {
            JumbotronComp,
            FirstSection,
            SecondSection,
            ThirdSection,
            FourthSection
        }
    }
</script>

<style lang="scss" scoped>
    // Import file.scss
    @import '../style/mixin.scss';
    div{
        background-color: antiquewhite;
    }
    #container{
        @include center-x(60%);
    }
</style>