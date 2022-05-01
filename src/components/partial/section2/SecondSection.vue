<template>

    <section>

        <ImageComp />

        <ParagraphComp />

    </section>

</template>

<script>
    // Import components
    import ImageComp from './ImageComp.vue'
    import ParagraphComp from './ParagraphComp.vue';
    export default {
        name: 'SecondSection',

        components: {
            ImageComp,
            ParagraphComp
        }
    }
</script>

<style lang="scss" scoped>
    // import file.scss
    @import '../../../style/mixin.scss';

    section {
        @include flex(row, initial, center);
        padding: 100px 0;
    }
</style>