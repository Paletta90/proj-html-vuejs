<template>

    <div>

        <!-- Lista della navbar -->
        <ul>

            <li v-for="(elem, index) in arrayNavbar" :key="index">

                <!-- Nome del dropdown -->
                {{elem}}
                <!-- Icona di fianco -->
                <i class="fa-solid fa-chevron-down"></i>

            </li>

        </ul>

    </div>


</template>

<script>
    export default {
        name: 'NavbarComp',

        // Data
        data() {
            return {
                arrayNavbar: ['Home', 'Pages', 'Courses', 'Features', 'Blog', 'Shop']
            }
        }
    }
</script>

<style lang="scss" scoped>
    // Import file.scss
    @import '../../style/mixin.scss';
    @import '../../style/variabili.scss';

    ul {
        @include listHorizontal();

        li {
            // Flexo i nomi con le icone di lato
            @include flex(row, initial, center);
            color: $font-colorNavbar;
            font-size: $font-sizeNavbar;
            font-weight: 600;
            margin-right: 15px;
            cursor: pointer;

            i{
                margin-left: 5px;
                font-size: 0.5rem;
            }
        }
    }
</style>