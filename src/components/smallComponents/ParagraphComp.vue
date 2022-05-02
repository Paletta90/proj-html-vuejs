<template>

    <div>

        <p class="small-title">{{smallText}} <span>{{smallText2}}</span> </p>

        <h2>{{title}} <span class="textColor">{{colorText}}</span> {{title2}}</h2>
        <p class="paragraph">{{paragraph}}</p>

    </div>

</template>

<script>
    export default {
        name: 'TitleComp',

        props: {
            smallText: String,
            smallText2: String,
            title: String,
            title2: String,
            colorText: String,
            paragraph: String,
        }
    }
</script>

<style lang="scss" scoped>
    // Import file.scss
    @import '../../style/mixin.scss';
    @import '../../style/variabili.scss';

    // Small text
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

    .paragraph {
        margin-bottom: 25px;
    }
</style>