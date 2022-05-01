<template>

    <section>

        <!-- Immagini di sinistra -->
        <ImagesComp />

        <!-- paragrafo di destra -->
        <ParagraphComp />

    </section>

</template>

<script>

// Import component
import ImagesComp from './ImagesComp.vue'
import ParagraphComp from './ParagraphComp.vue'
export default {
    name: 'FifthSection',

    components:{
        ImagesComp,
        ParagraphComp
    }
}
</script>

<style lang="scss" scoped>

    section{
        padding: 50px 0;
        display: flex;
    }

</style>