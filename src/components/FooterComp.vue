<template>

    <div id="footer">

        <InfoComp :info="info" :explore="explore" :information="information"/>

        <div class="text-center">&#x000A9; 2020 Maxcoach. All Rights Reserved</div>

        <div class="scroll-up" @click="scrollToTop"><i class="fa-solid fa-arrow-up"></i></div>
    </div>

</template>

<script>
    // import components
    import InfoComp from './partial/footer/InfoComp.vue'

    export default {
        name: 'FooterComp',

        components: {
            InfoComp
        },

        data() {
            return {
                info: ['382 NE 191st # 87394 Miami, FL 33179-3899', '+1(305)547-9909', '(9am - 5pm EST, Monday-Friday)', 'support@maxcoach'],

                explore: ['Start here', 'Blog', 'About us', 'Success story', 'Courses', 'Contact us'],

                information: ['Membership', 'Purchase guide', 'Privacy policy', 'Terms of service']
            }
        },

        methods:{
            scrollToTop(){
                window.scrollTo({
                    top: 0,
                    behavior: 'smooth'
                });
            }
        }
    }
</script>

<style lang="scss" scoped>

    // import file.scss
    @import '../style/mixin.scss';
    @import '../style/variabili.scss';

    #footer{
        @include center-x(80%);
        padding: 50px 0;
        color: $color-stormDust;
        position: relative;
    }
    .text-center{
        margin-top: 50px;
    }
    .scroll-up{
        width: 50px;
        height: 50px;
        border-radius: 50%;
        @include flex(row, center, center);
        background-color: $color-mountainMeadow;
        position: absolute;
        right: 0;
        bottom: 10%;
        cursor: pointer;
        i{
            color: white;
        }
    }
</style>