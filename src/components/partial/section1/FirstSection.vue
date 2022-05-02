<template>

    <section>

        <div class="block">

            <ParagraphComp />

            <ImageComp />

        </div>

        <StatisticComp />

    </section>

</template>

<script>
    // Import components
    import ParagraphComp from './ParagraphComp.vue'
    import ImageComp from './ImageComp.vue'
    import StatisticComp from './StatisticComp.vue'

    export default {
        name: 'FirstSection',

        components: {
            ParagraphComp,
            ImageComp,
            StatisticComp
        }
    }
</script>

<style lang="scss" scoped>
    // import file.scss
    @import '../../../style/variabili.scss';
    @import '../../../style/mixin.scss';

    section {
        @include center-x(60%);
        padding: 100px 0;

        .block{
            width: 100%;
            display: flex;
        }
    }
</style>