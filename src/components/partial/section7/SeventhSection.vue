<template>

    <section>

        <!-- Titolo -->
        <div class="text-center">

            <TitleComp :title="title" :colorText="colorText" :paragraph="paragraph" />

        </div>

        <!-- Input e button -->
        <div>

            <input type="text" placeholder="Enter your email">
            <button>Subscribe</button>

        </div>

        <!-- Immagini da spostare con position -->
        <img src="../../../assets/background/maxcoach-shape-02.png" alt="Semicerchio" width="25%">
        <img src="../../../assets/background/maxcoach-shape-08.png" alt="Griglia punteggiata" width="25%">
        <div class="circle"></div>
    </section>

</template>

<script>
    // import components
    import TitleComp from '../../smallComponents/TitleComp.vue'
    export default {
        name: 'SeventhSection',

        components: {
            TitleComp
        },

        data() {
            return {
                // TitleComp
                title: 'Subscribe',
                colorText: 'Newsletters',
                paragraph: 'Enter your email address to register to our newsletter subscription delivered on a regular basis!'
            }
        }
    }
</script>

<style lang="scss" scoped>
    // import file.scss
    @import '../../../style/mixin.scss';
    @import '../../../style/variabili.scss';

    section {
        @include center-x(50%);
        position: relative;
        padding: 50px 0;

        div:nth-of-type(2) {
            display: flex;

            input {
                width: 100%;
            }

            input,
            button {
                padding: 15px;
                border: none;
            }

            input {
                background-color: $color-quillGray;
                border-radius: 5px 0 0 5px
            }

            button {
                background-color: $color-mountainMeadow;
                border-radius: 0 5px 5px 0;
            }

        }

        img {
            position: absolute;
        }

        // Semicerchio
        img:nth-of-type(1) {
            bottom: 20%;
            left: 125%;
        }
        // Griglia
        img:nth-of-type(2) {
            bottom: 40%;
            left: 120%;
            transform: rotate(30deg);
        }
        .circle{
            border-color: $color-mountainMeadow!important;
            position: absolute;
            bottom: 25%;
            right: 160%;
        }
    }
</style>