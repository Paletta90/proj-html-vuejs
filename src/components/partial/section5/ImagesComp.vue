<template>

    <div id="contenitore">

            <img src="../../../assets/image/home-3-team-image.png" alt="Tre immagini di volti" width="100%">
            <img src="../../../assets/background/maxcoach-shape-05.png" alt="Rombo punteggiato" width="25%">
            <img src="../../../assets/background/maxcoach-shape-07.png" alt="Griglia punteggiata" width="25%">
            <img src="../../../assets/background/maxcoach-shape-01.png" alt="Linee colorate" width="25%">
            <div class="circle"></div>

    </div>


</template>

<script>
    export default {
        name: 'ImageComp'
    }
</script>

<style lang="scss" scoped>

    #contenitore {
        width: calc(60% - 50px);
        margin-right: 50px;
        position: relative;

        img:nth-of-type(1){
            position: relative;
            z-index: 1;
        }
        // Rombo
        img:nth-of-type(2) {
            position: absolute;
            top: 30%;
            left: 0%;
            transform: translate(-50%, 0);
            z-index: 0;
        }
        
        // Griglia
        img:nth-of-type(3) {
            position: absolute;
            right: 34%;
            bottom: 0%;
            transform: translate(0, +60%);
            z-index: 0;
        }
        // Linee colorate
        img:nth-of-type(4) {
            position: absolute;
            bottom: 0%;
            right: 125%;
            z-index: 0;
        }
        // Cerchio colorato
        .circle{
            position: absolute;
            top: 0%;
            left: 100%;
        }
        
    }

</style>