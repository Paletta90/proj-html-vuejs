<template>

    <div id="contenitore">

        <!-- Immagina sinistra -->
        <div class="card" v-for="(elem, index) in cards" :key="index">

            <div>
                <!-- Immagine -->
                <img :src="require(`../../assets/image/${String(elem.image)}`)" alt="" width="100%">

                <!-- Prezzo -->
                <p v-if="elem.type == 'course'" class="price">{{elem.price}}<span
                        style="font-size: 0.8rem">{{elem.rest}}</span> </p>
                <p v-if="elem.type == 'blog'" class="textType">{{elem.price}}</p>

                <!-- Descrizione -->
                <p class="description">{{elem.description}}</p>

            </div>

            <div class="paragraph">

                <!-- Studenti -->
                <p><i :class="elem.iconLesson"></i> {{elem.lessons}}</p>

                <!-- Lezioni -->
                <p><i :class="elem.iconUser"></i> {{elem.students}}</p>

            </div>



        </div>

    </div>

</template>

<script>
    export default {
        name: 'ThreeCard',

        props: {
            cards: []
        }
    }
</script>

<style lang="scss" scoped>
    // import file.scss
    @import '../../style/variabili.scss';
    @import '../../style/mixin.scss';

    #contenitore {
        width: 100%;
        display: flex;

        .card {
            width: calc((100% / 3) - 20px);
            @include flex(column, space-between, initial);
            margin: 0 10px;
            cursor: pointer;

            // Hover sulla card: la scritta si colora
            &:hover {
                .description {
                    color: $color-mountainMeadow;
                }

            }

            img{
                margin-bottom: 10px;
            }
            // prezzo
            .price {
                @include font(initial, 700, $color-mountainMeadow);
                margin-bottom: 10px;
            }

            .textType {
                @include font($font-sizeNavbar, 500, $color-gunSmoke);
                text-transform: uppercase;
                margin-bottom: 10px;
            }

            // Descrizione
            .description {
                font-weight: 800;
            }

            // Dati
            .paragraph {
                display: flex;
                margin-top: 20px;

                p {
                    margin-right: 10px
                }
            }
        }

    }
</style>