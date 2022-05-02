<template>

    <section>

        <!-- Paragrafo di sinistra -->
        <div class="paragrafo">

            <ParagraphComp :smallText="smallText" :title="title" :colorText="colorText" :paragraph="paragraph"
                :title2="title2" />

            <p class="textBold">View All <i class="fa-solid fa-right-long"></i></p>

        </div>


        <!-- Parte di destra recensioni -->
        <ReviewComp />

    </section>

</template>

<script>
    // Import Components
    import ReviewComp from './ReviewComp.vue'
    import ParagraphComp from '../../smallComponents/ParagraphComp.vue'

    export default {
        name: 'FourthSection',

        components: {
            ParagraphComp,
            ReviewComp
        },

        data() {
            return {
                smallText: 'testimonials',
                title: 'Why do people',
                title2: 'Us',
                colorText: '*Hearts*',
                paragraph: 'Seeking for verbals of our service quality? Find theme here. Everything is trasparent and straghtforward fro your sense of justification'
            }
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

        .paragrafo {
            width: calc(40% - 25px);
            margin-right: 25px;

            // View All
            .textBold {
                text-decoration: underline;
                cursor: pointer;
            }
        }
    }
</style>