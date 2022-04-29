<template>

    <!-- Descrizione di sinistra -->
    <div>

        <p>Everything in <span>maxcoach</span></p>

        <h2>Learn about out <span>Work Culture</span> at MaxCoach</h2>

        <p>Spend some time to visit out website or head office and discover out current courses, enrollment
            procedure, and registration deadline. We're opening new classes every beginning of each month</p>

        <p>Have a questions? <span>Get Free guide <i class="fa-solid fa-right-long"></i></span></p>

    </div>

</template>

<script>
    export default {
        name: 'ParagraphComp'
    }
</script>

<style lang="scss" scoped>
    // import file.scss
    @import '../../../style/variabili.scss';

    div {

        width: calc(40% - 25px);
        margin-right: 25px;

        // MaxCoach
        p:nth-of-type(1) {

            font-weight: 500;
            color: $color-gunSmoke;
            text-transform: uppercase;
            margin-bottom: 15px;

            span {
                color: $color-stormDust;
                font-weight: 700;
            }

        }

        // Titolo
        h2 {
            font-size: $font-titleh2;
            margin-bottom: 10px;

            span {
                color: $color-mountainMeadow;
            }
        }

        // Testo del paragrafo
        p:nth-of-type(2) {
            font-size: $font-sizeNavbar;
            font-weight: 500;
            line-height: 20px;
            color: $color-gunSmoke;
            margin-bottom: 25px;
        }

        // Have a question?
        p:nth-of-type(3) {
            font-size: $font-sizeNavbar;
            font-weight: 500;
            color: $color-stormDust;

            span {
                font-size: $font-sizeNavbar;
                font-weight: 700;
                color: $color-mountainMeadow;
                text-decoration: underline;
                text-decoration-color: $color-gunSmoke;
            }
        }

    }
</style>