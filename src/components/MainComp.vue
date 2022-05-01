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

            <!-- Quinta sezione -->
            <FifthSection />

            <!-- Sesta sezione -->
            <SixthSection />

            <!-- Settima sezione -->
            <SeventhSection />

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
    import FifthSection from './partial/section5/FifthSection.vue'
    import SixthSection from './partial/section6/SixthSection.vue'
    import SeventhSection from './partial/section7/SeventhSection.vue'

    export default {
        name: 'MainComp',

        components: {
            JumbotronComp,
            FirstSection,
            SecondSection,
            ThirdSection,
            FourthSection,
            FifthSection,
            SixthSection,
            SeventhSection
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