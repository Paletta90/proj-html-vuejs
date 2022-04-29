<template>

    <!-- Descrizione di destra -->
    <div>
        
        <p>How we work</p>

        <h2>Upgrade Your Skills <span>Upgrade Your Life</span></h2>

        <p>Opening up more oppurtunities in front of you to get the ticket to more enjoyable door in life. Getting
            equipped with new skills for new sets on insights into your carrer. MaxCoach accompany learners in every
            stage of learning</p>

        <p>Download free guidebook <i class="fa-solid fa-right-long"></i></p>

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
    @import '../../../style/mixin.scss';

    div {
        width: 40%;

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
                font-weight: 100;
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
            font-weight: 1000;
            text-decoration: underline;
            color: $color-stormDust;

        }

    }
</style>