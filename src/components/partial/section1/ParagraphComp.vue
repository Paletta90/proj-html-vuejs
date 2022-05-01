<template>

    <!-- Descrizione di sinistra -->
    <div id="contenitore">

        <TitleComp :smallText="smallText" :smallText2="smallText2" :title="title" :colorText="colorText"
            :paragraph="paragraph" :title2="title2" />

        <p>Have a questions? <span>Get Free guide <i class="fa-solid fa-right-long"></i></span></p>

    </div>

</template>

<script>
    // Import Components
    import TitleComp from '../../smallComponents/TitleComp.vue'

    export default {
        name: 'ParagraphComp',

        components:{
            TitleComp
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

    #contenitore {

        width: calc(40% - 25px);
        margin-right: 25px;

        // Have a question?
        p{
            @include font($font-sizeNavbar, 500, $color-stormDust);

            span {
                @include font($font-sizeNavbar, 700, $color-mountainMeadow);
                text-decoration: underline;
                text-decoration-color: $color-gunSmoke;
            }
        }

    }
</style>