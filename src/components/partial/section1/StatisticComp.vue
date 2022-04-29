<template>

    <!-- Statistiche -->
    <div class="block-statistic">

        <div>

            <div>129 &#x0002B;</div>
            <p>enrolled leaners</p>

        </div>

        <div>

            <div>80</div>
            <p>finished sessions</p>

        </div>

        <div>

            <div>4 &#x00025;</div>
            <p>satisfaction rate</p>

        </div>

    </div>

</template>

<script>
export default {
    name: 'StatisticComp'
}
</script>

<style lang="scss" scoped>
    // import file.scss
    @import '../../../style/mixin.scss';
    @import '../../../style/variabili.scss';

    .block-statistic{
        width: 100%;
        @include flex(row, space-around, initial);
        margin-top: 100px;

        div:nth-child(1),
        div:nth-child(2),
        div:nth-child(3){
            @include flex(column, center, center);

            div{
                font-size: $font-statistic;
                font-weight: 1000;
                color: $color-mountainMeadow;
                margin-bottom: 20px;
            }
            p{
                text-transform: uppercase;
                color: $color-gunSmoke;
                font-weight: 700;
            }
        }

    }
</style>