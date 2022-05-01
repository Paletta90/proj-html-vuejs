<template>

    <!-- Descrizione di destra -->
    <div id="contenitore">
        
        <TitleComp :smallText="smallText" :title="title" :colorText="colorText" :paragraph="paragraph"/>

        <p class="textBold">Download free guidebook <i class="fa-solid fa-right-long"></i></p>

    </div>

</template>

<script>
    // import components
    import TitleComp from '../../smallComponents/TitleComp.vue'

    export default {
        name: 'ParagraphComp',

        components:{
            TitleComp
        },

        data(){
            return{
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
    @import '../../../style/variabili.scss';
    @import '../../../style/mixin.scss';

    #contenitore{
        width: 40%;

        // Download free
        .textBold {
            text-decoration: underline;
        }

    }
</style>