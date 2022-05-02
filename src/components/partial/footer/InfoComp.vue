<template>

    <div id="contenitore">

        <!-- Lista di sinisra -->
        <div>

            <!-- Lista contatti -->
            <h4>Address</h4>
            <ul>
                <li v-for="(elem, index) in info" :key="index">{{elem}}</li>
            </ul>

            <div class="icons">
               <a href="#"><svg xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 64 64" width="64px" height="64px"><path d="M48,7H16c-4.418,0-8,3.582-8,8v32c0,4.418,3.582,8,8,8h17V38h-6v-7h6v-5c0-7,4-11,10-11c3.133,0,5,1,5,1v6h-4 c-2.86,0-4,2.093-4,4v5h7l-1,7h-6v17h8c4.418,0,8-3.582,8-8V15C56,10.582,52.418,7,48,7z"/></svg></a> 
                <a href="#"><svg xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 64 64" width="64px" height="64px"><path d="M61.932,15.439c-2.099,0.93-4.356,1.55-6.737,1.843c2.421-1.437,4.283-3.729,5.157-6.437	c-2.265,1.328-4.774,2.303-7.444,2.817C50.776,11.402,47.735,10,44.366,10c-6.472,0-11.717,5.2-11.717,11.611	c0,0.907,0.106,1.791,0.306,2.649c-9.736-0.489-18.371-5.117-24.148-12.141c-1.015,1.716-1.586,3.726-1.586,5.847	c0,4.031,2.064,7.579,5.211,9.67c-1.921-0.059-3.729-0.593-5.312-1.45c0,0.035,0,0.087,0,0.136c0,5.633,4.04,10.323,9.395,11.391	c-0.979,0.268-2.013,0.417-3.079,0.417c-0.757,0-1.494-0.086-2.208-0.214c1.491,4.603,5.817,7.968,10.942,8.067	c-4.01,3.109-9.06,4.971-14.552,4.971c-0.949,0-1.876-0.054-2.793-0.165C10.012,54.074,16.173,56,22.786,56	c21.549,0,33.337-17.696,33.337-33.047c0-0.503-0.016-1.004-0.04-1.499C58.384,19.83,60.366,17.78,61.932,15.439"/></svg></a>
                <a href="#"><svg xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 50 50" width="50px" height="50px"><path d="M 16 3 C 8.8324839 3 3 8.8324839 3 16 L 3 34 C 3 41.167516 8.8324839 47 16 47 L 34 47 C 41.167516 47 47 41.167516 47 34 L 47 16 C 47 8.8324839 41.167516 3 34 3 L 16 3 z M 16 5 L 34 5 C 40.086484 5 45 9.9135161 45 16 L 45 34 C 45 40.086484 40.086484 45 34 45 L 16 45 C 9.9135161 45 5 40.086484 5 34 L 5 16 C 5 9.9135161 9.9135161 5 16 5 z M 37 11 A 2 2 0 0 0 35 13 A 2 2 0 0 0 37 15 A 2 2 0 0 0 39 13 A 2 2 0 0 0 37 11 z M 25 14 C 18.936712 14 14 18.936712 14 25 C 14 31.063288 18.936712 36 25 36 C 31.063288 36 36 31.063288 36 25 C 36 18.936712 31.063288 14 25 14 z M 25 16 C 29.982407 16 34 20.017593 34 25 C 34 29.982407 29.982407 34 25 34 C 20.017593 34 16 29.982407 16 25 C 16 20.017593 20.017593 16 25 16 z"/></svg></a>
                <a href="#"><svg xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 50 50" width="50px" height="50px"><path d="M41,4H9C6.24,4,4,6.24,4,9v32c0,2.76,2.24,5,5,5h32c2.76,0,5-2.24,5-5V9C46,6.24,43.76,4,41,4z M17,20v19h-6V20H17z M11,14.47c0-1.4,1.2-2.47,3-2.47s2.93,1.07,3,2.47c0,1.4-1.12,2.53-3,2.53C12.2,17,11,15.87,11,14.47z M39,39h-6c0,0,0-9.26,0-10 c0-2-1-4-3.5-4.04h-0.08C27,24.96,26,27.02,26,29c0,0.91,0,10,0,10h-6V20h6v2.56c0,0,1.93-2.56,5.81-2.56 c3.97,0,7.19,2.73,7.19,8.26V39z"/></svg></a>
            </div>

        </div>

        <!-- Lista di destra -->
        <div class="block-right">

            <!-- List explore -->
            <div>
                <h4>Explore</h4>
                <ul>
                    <li v-for="(elem, index) in explore" :key="index"><a href="#">{{elem}}</a></li>
                </ul>
            </div>

            <!-- List information -->
            <div>
                <h4>Information</h4>
                <ul>
                    <li v-for="(elem, index) in information" :key="index"><a href="#">{{elem}}</a></li>
                </ul>
            </div>

        </div>

    </div>

</template>

<script>
    export default {
        name: 'AddressComp',

        props: {
            info: [],
            explore: [],
            information: []
        }
    }
</script>

<style lang="scss" scoped>

    // import file.scss
    @import '../../../style/mixin.scss';
    @import '../../../style/variabili.scss';

    #contenitore{
        @include flex(row, space-between, initial);
    }
    h4 {
        color: white;
        margin-bottom: 25px;
    }

    ul {
        list-style-type: none;

        li {
            margin-bottom: 15px;
            
            a{
                color: $color-stormDust;
                text-decoration: none;

                &:hover{
                    text-decoration: underline;
                }
            }
        }
    }
    svg{
        width: 40px;
        fill: $color-stormDust;
        margin-right: 10px;
    }
    .icons{
        @include flex(row, initial, center)
    }
    .block-right{
        @include flex(row, space-between, initial);
        width: 40%;
    }
</style>