<template>

    <!-- Blocco immagine sinistra -->
    <div>

        <img src="../../../assets/image/stock-full-hd-11-670x450.jpg" alt="ragazza al telefono" width="100%">
        <img src="../../../assets/icon/icon-youtube-play.png" alt="Icona youtube" width="15%">
        <img src="../../../assets/background/maxcoach-shape-05-100x100.png" alt="Rombo punteggiato" width="20%">
        <img src="../../../assets/background/maxcoach-shape-07-100x100.png" alt="Griglia punteggiata" width="20%">
        <div class="circle"></div>

    </div>

</template>

<script>
export default {
    name: 'ImageComp'
}
</script>

<style lang="scss" scoped>

    div{
        width: calc(60% - 50px);
        position: relative;
        margin-right: 50px;

        // Icona youtube
        img:nth-of-type(2){
            position: absolute;
            left: 50%;
            top: 50%;
            transform: translate(-50%, -50%);
        }

        // Rombo punteggiato
        img:nth-of-type(3){
            position: absolute;
            right: 100%;
            transform: translate(50%, 15%);
            z-index: -1;
        }

        // Griglia punteggiata
        img:nth-of-type(4){
            position: absolute;
            top: 100%;
            transform: translate(-80%, -40%);
            z-index: -1;
        }

        .circle{
            position: absolute;
            bottom: 100%;
            left: 110%;
            z-index: -1;
        }
    }

</style>