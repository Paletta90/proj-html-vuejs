<template>

    <section>

        <ImageComp />

        <!-- Descrizione di destra -->
        <div class="paragrafo">

            <ParagraphComp :smallText="smallText" :title="title" :colorText="colorText" :paragraph="paragraph" />

            <p class="textBold">Download free guidebook <i class="fa-solid fa-right-long"></i></p>

        </div>

    </section>

</template>

<script>
    // Import components
    import ParagraphComp from '../../smallComponents/ParagraphComp.vue'
    import ImageComp from './ImageComp.vue'

    export default {
        name: 'SecondSection',

        components: {
            ImageComp,
            ParagraphComp
        },

        data() {
            return {
                smallText: 'how we work',
                title: 'Upgrade Your Skills',
                colorText: 'Upgrade Your Life',
                paragraph: 'Opening up more oppurtunities in front of you to get the ticket to more enjoyable door in life. Getting equipped with new skills for new sets on insights into your carrer. MaxCoach accompany learners in every stage of learning'
            }
        }
    }
</script>

<style lang="scss" scoped>
    // import file.scss
    @import '../../../style/mixin.scss';

    section {
        @include center-x(60%);
        @include flex(row, initial, center);
        padding: 100px 0;

        .paragrafo {
            width: 40%;

            // Download free
            .textBold {
                text-decoration: underline;
            }

        }
    }
</style>