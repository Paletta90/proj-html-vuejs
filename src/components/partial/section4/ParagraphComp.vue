<template>

    <!-- Paragrafo di sinistra -->
    <div id="contenitore">

        <TitleComp :smallText="smallText" :title="title" :colorText="colorText" :paragraph="paragraph"
            :title2="title2" />

        <p class="textBold">View All <i class="fa-solid fa-right-long"></i></p>

    </div>

</template>

<script>
    // import components
    import TitleComp from '../../smallComponents/TitleComp.vue'
    export default {
        name: 'ParagraphComp',

        components: {
            TitleComp
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

    #contenitore {
        width: calc(40% - 25px);
        margin-right: 25px;
    }

    // Download free
    .textBold {
        text-decoration: underline;
    }

</style>