<template>

    <!-- Immagine logo MaxCoach -->
    <div>

        <img src="../../../assets/loghi/dark-logo.png" alt="immagine logo MaxCoach" width="150px">

    </div>

</template>

<script>
export default {
    name: 'LogoComp'
}
</script>

<style lang="scss" scoped>

    // Import file.scss
    @import '../../../style/mixin.scss';

    div{
        // Flexo il logo per centrarlo
        @include flex(row, center, initial);
        cursor: pointer;
    }

</style>