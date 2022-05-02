<template>

    <section>

        <!-- Paragrafo e immagine -->
        <div class="block">

            <!-- Descrizione di sinistra -->
            <div class="paragrafo">

                <ParagraphComp :smallText="smallText" :smallText2="smallText2" :title="title" :colorText="colorText"
                    :paragraph="paragraph" :title2="title2" />

                <p class="paragraph">Have a questions? <span>Get Free guide <i
                            class="fa-solid fa-right-long"></i></span></p>

            </div>

            <!-- Immagine di destra -->
            <ImageComp />

        </div>

        <!-- Statistiche centrali -->
        <StatisticComp />

    </section>

</template>

<script>
    // Import components
    import ParagraphComp from '../../smallComponents/ParagraphComp.vue'
    import ImageComp from './ImageComp.vue'
    import StatisticComp from './StatisticComp.vue'

    export default {
        name: 'FirstSection',

        components: {
            ParagraphComp,
            ImageComp,
            StatisticComp
        },

        data() {
            return {
                smallText: 'everything in ',
                smallText2: 'maxcoach',
                title: 'Learn about out ',
                colorText: 'Work Culture',
                title2: 'at MaxCoach',
                paragraph: 'Spend some time to visit out website or head office and discover out current courses, enrollment procedure, and registration deadline. We re opening new classes every beginning of each month'
            }
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

        .block {
            width: 100%;
            display: flex;

            .paragrafo {

                width: calc(40% - 25px);
                margin-right: 25px;

                // Have a question?
                .paragraph {
                    span {
                        @include font($font-sizeNavbar, 700, $color-mountainMeadow);
                        text-decoration: underline;
                        text-decoration-color: $color-gunSmoke;
                        cursor: pointer;
                    }
                }

            }
        }
    }
</style>