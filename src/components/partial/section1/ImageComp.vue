<template>
    <!-- Immagine di destra -->
    <div class="block-right">

        <div class="circle"></div>

        <div>

            <img src="../../../assets/background/maxcoach-shape-07-100x100.png" alt="Griglia punteggiata" width="25%">
            <img src="../../../assets/image/about-us-01-ohkia3qg98rq9vg3s0mn2hkflr1migdqdw370qnegc.jpg"
                alt="Ragazza davanti un pc" width="25%">
            <img src="../../../assets/image/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg"
                alt="Work ambient" width="100%">
            <img src="../../../assets/background/maxcoach-shape-02.png" alt="Semicerchio" width="20%">

        </div>

    </div>
    
</template>

<script>
    export default {
        name: 'ImageComp'
    }
</script>

<style lang="scss" scoped>
    // import file.scss
    @import '../../../style/variabili.scss';

    .block-right {
        width: calc(60% - 100px);
        margin-left: 100px;
        position: relative;

        .circle {
            width: 55px;
            height: 55px;
            border-radius: 50%;
            border: 7px solid $color-texasRose;
            position: absolute;
            left: -35%;
        }


        img {
            position: absolute;
        }

        // Immagine griglia punteggiata
        img:nth-of-type(1) {
            left: 100%;
            transform: translate(-75%, -50%);
        }

        // Immagine ragazza davanti pc
        img:nth-of-type(2) {
            z-index: 1;
            left: 100%;
            transform: translate(-50%, -50%);
        }

        // Semicerchio
        img:nth-of-type(4) {
            z-index: 1;
            left: 75%;
            transform: translate(-50%, 290%);
        }
    }
</style>