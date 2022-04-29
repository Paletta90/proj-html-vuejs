<template>

    <div>

        <p class="small-title">{{smallText}}</p>

        <h2>{{title}} <span class="textColor">{{colorText}}</span></h2>

    </div>

</template>

<script>
    export default {
        name: 'TitleComp',

        props: {
            smallText: String,
            title: String,
            colorText:String
        }
    }
</script>

<style lang="scss" scoped>
    // Import file.scss
    @import '../../style/mixin.scss';
    @import '../../style/variabili.scss';

    // Titolo
    h2 {
        font-size: $font-titleh2;
        margin-bottom: 10px;
    }
</style>