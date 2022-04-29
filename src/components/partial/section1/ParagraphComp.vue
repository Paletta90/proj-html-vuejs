<template>

    <!-- Descrizione di sinistra -->
    <div>

        <p class="small-title">Everything in <span>maxcoach</span></p>

        <h2>Learn about out <span class="textColor">Work Culture</span> at MaxCoach</h2>

        <p class="paragraph">Spend some time to visit out website or head office and discover out current courses, enrollment
            procedure, and registration deadline. We're opening new classes every beginning of each month</p>

        <p>Have a questions? <span>Get Free guide <i class="fa-solid fa-right-long"></i></span></p>

    </div>

</template>

<script>
    export default {
        name: 'ParagraphComp',

    }
</script>

<style lang="scss" scoped>
    // import file.scss
    @import '../../../style/variabili.scss';
    @import '../../../style/mixin.scss';

    div {

        width: calc(40% - 25px);
        margin-right: 25px;

        // MaxCoach
        .small-title {

            span {
                @include font(initial, 700, $color-stormDust);
            }

        }

        // Titolo
        h2 {
            font-size: $font-titleh2;
            margin-bottom: 10px;
        }

        // Testo del paragrafo
        .paragraph {
            margin-bottom: 25px;
        }

        // Have a question?
        p:nth-of-type(3) {
            @include font($font-sizeNavbar, 500, $color-stormDust);

            span {
                @include font($font-sizeNavbar, 700, $color-mountainMeadow);
                text-decoration: underline;
                text-decoration-color: $color-gunSmoke;
            }
        }

    }
</style>