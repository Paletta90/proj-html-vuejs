<template>

    <section>

        <!-- Immagini di sinistra -->
        <ImagesComp />

        <div class="paragrafo">

            <div class="circle"></div>

            <ParagraphComp :smallText="smallText" :smallText2="smallText2" :title="title" :colorText="colorText"
                :paragraph="paragraph" :title2="title2" />

            <span>
                Get Free Guide
            </span>

        </div>

    </section>

</template>

<script>
    // Import component
    import ImagesComp from './ImagesComp.vue'
    import ParagraphComp from '../../smallComponents/ParagraphComp.vue'
    export default {
        name: 'FifthSection',

        components: {
            ImagesComp,
            ParagraphComp
        },

        data() {
            return {
                smallText: 'everything in ',
                smallText2: 'maxcoach',
                title: 'We`re Here To',
                colorText: 'Transform',
                title2: 'you',
                paragraph: 'As learners, people con enjoy great companionship from MaxCoach mentors and educators. We can help you develop and grow at your best'
            }
        }
    }
</script>

<style lang="scss" scoped>
    // Import componets
    @import '../../../style/mixin.scss';
    @import '../../../style/variabili.scss';

    section {
        @include center-x(60%);
        @include flex(row, initial, center);
        padding: 50px 0;

        .paragrafo {
            width: 40%;
            position: relative;

            .circle{
                position: absolute;
                bottom: 120%;
            }
            span {
            padding: 15px 40px;
            border-radius: 5px;
            background-color: $color-mountainMeadow;
            @include font(initial, 700, white);
            cursor: pointer;

            &:hover {
                background-color: $color-quillGray;

                color: $color-mountainMeadow;
            }
        }
        }

    }
</style>