<template>

    <section>

        <!-- Titolo 1 -->
        <h2>Commence Business</h2>

        <!-- Titolo 2 -->
        <h1>Distant Mentoring Program</h1>

        <!-- Button -->
        <div class="button">
            <p>Download free guidebook <i class="fa-solid fa-right-long"></i></p>
        </div>

    </section>

</template>

<script>

    export default {
        name: 'JumbotronComp'
    }

</script>

<style lang="scss" scoped>

    // import file.scss
    @import '../../../style/mixin.scss';
    @import '../../../style/variabili.scss';

    section {
        height: 70vh;
        background-image: url('../../../assets/image/jumbotron.jpg');
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
        // Flexo i titoli e il button al centro del jumbotron
        @include flex(column, center, center);

        h2{
            color: white;
            margin-bottom: 15px;
        }
        h1{
            color: white;
            font-weight: 100;
            font-size: $font-titleh1;
            margin-bottom: 15px;
        }

        .button{
            padding: 15px 20px;
            border-radius: 5px;
            background-color: white;
            font-weight: 800;
            color: $color-mountainMeadow;
            cursor: pointer;

            &:hover{
                background-color: $color-mountainMeadow;
                color: white;
            }
        }
    }
</style>