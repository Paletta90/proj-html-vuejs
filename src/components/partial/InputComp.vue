<template>

    <div>

        <!-- Icona carrello e profilo -->
        <div class="icons">

            <!-- Icona carrello -->
            <div class="carrello">
                <i class="fa-solid fa-cart-shopping"></i>
                <div class="circle-basket">0</div>
            </div>


            <!-- Icona profilo -->
            <i class="fa-regular fa-circle-user"></i>

        </div>

        <!-- Input -->
        <div class="form-group">

            <!-- Input di testo -->
            <input type="text" placeholder="Search">

            <!-- Icona dentro l'input -->
            <button type="submit"><i class="fa-solid fa-magnifying-glass"></i></button>

        </div>

    </div>

</template>

<script>
    export default {
        name: 'InputComp'
    }
</script>

<style lang="scss" scoped>

    // Import file.scss
    @import '../../style/mixin.scss';
    @import '../../style/variabili.scss';

    div {

        // Flexo le icone e l'input
        @include flex(row, flex-end, center);

        .icons {
            
            margin-right: 15px;

            .carrello{
                position: relative;
                margin-right: 15px;
            }
            .circle-basket{
                width: 15px;
                height: 15px;
                font-size: 10px;
                border-radius: 50%;
                background-color: $color-mountainMeadow;
                color: white;

                // Centro il numero dentro al cerchio
                @include flex(row, center, center);

                // Con position metto il cerchio in alot a destra del carrello
                position: absolute;
                bottom: 12px;
                left: 12px;
            }
        }

        .form-group {
            position: relative;

            input {
                width: 100%;
                display: block;
                padding: 10px;
                border: none;
                border-radius: 10px;
                background-color: $color-quillGray;
            }

            button {
                background: transparent;
                border: none;
                cursor: pointer;
                display: inline-block;
                font-size: 20px;
                position: absolute;
                top: 0;
                right: 0;
                padding: 7px 20px;

                i {
                    color: $color-mountainMeadow;
                }
            }
        }
    }
</style>