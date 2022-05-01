<template>

    <div id="contenitore">

        <TitleComp x="x" :smallText="smallText" :smallText2="smallText2" :title="title" :colorText="colorText"
            :paragraph="paragraph" :title2="title2" />

        <span>
           Get Free Guide 
        </span>

    </div>

</template>

<script>
    // Import component
    import TitleComp from '../../../components/smallComponents/TitleComp.vue'

    export default {
        name: 'ParagraphComp',

        components: {
            TitleComp
        },

        data() {
            return {
                x: '&#x00027;',
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

// Import file.scss
@import '../../../style/variabili.scss';
@import '../../../style/mixin.scss';
    #contenitore {
        width: 40%;
    }

    span{
        padding: 15px 40px;
        border-radius: 5px;
        background-color: $color-mountainMeadow;
        @include font(initial, 700, white)
    }
</style>