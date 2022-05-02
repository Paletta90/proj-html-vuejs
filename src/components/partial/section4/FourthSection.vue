<template>

    <section>

        <!-- Parte di sinistra -->
        <ParagraphComp />

        <!-- Parte di destra recensioni -->
        <ReviewComp />

    </section>

</template>

<script>

    // Import Components
    import ParagraphComp from './ParagraphComp.vue'
    import ReviewComp from './ReviewComp.vue'

    export default {
        name: 'FourthSection',

        components: {
            ParagraphComp,
            ReviewComp
        }
    }
</script>

<style lang="scss" scoped>
    // import file.scss
    @import '../../../style/mixin.scss';
    @import '../../../style/variabili.scss';

    section {
        @include center-x(60%);
        @include flex(row, initial, center);
        padding: 50px 0;
    }

</style>