<template>

    <div>

        <!-- Lista della navbar -->
        <ul>

            <li v-for="(elem, index) in arrayNavbar" :key="index">

                <!-- Nomi del menu -->
                <a href="#">{{elem}}</a>
                <!-- Icona di fianco -->
                <i class="fa-solid fa-chevron-down"></i>

            </li>

        </ul>

    </div>


</template>

<script>
    export default {
        name: 'NavbarComp',

        props:{
            arrayNavbar: []
        }
    }
</script>

<style lang="scss" scoped>
    // Import file.scss
    @import '../../../style/mixin.scss';
    @import '../../../style/variabili.scss';

    ul {
        @include listHorizontal();

        li {
            @include flex(row, initial, center);
            margin-right: 15px;
            a{
                @include font($font-sizeNavbar, 600, $font-colorNavbar);
                text-decoration: none;

                &:hover{
                    text-decoration: underline;
                }
            }
            i{
                margin-left: 5px;
                font-size: 0.5rem;
            }
        }
    }
</style>