<template>

    <section>

        <div class="text-center">
            <TitleComp :smallText="smallText" :title="title" :colorText="colorText" />
        </div>

        <ThreeCard :cards="this.cards" />

        <div class="wave">

            <div>
                <!-- Lista di pallini -->
                <div class="list-circle">
                    <div class="small-circle" style="background-color: "></div>
                    <div class="small-circle"></div>
                    <div class="small-circle"></div>
                    <div class="small-circle"></div>
                    <div class="small-circle"></div>
                </div>

                <!-- View All courses -->
                <p class="paragraph">Control your personal preference settings to get notified about appropriate
                    courses.
                    <span class="textBold">View all
                        courses <i class="fa-solid fa-right-long"></i></span></p>
            </div>


        </div>
    </section>

</template>

<script>
    // Import components
    import TitleComp from '../../smallComponents/TitleComp.vue'
    import ThreeCard from './ThreeCard.vue'

    export default {
        name: 'ThirdSection',

        components: {
            TitleComp,
            ThreeCard,
        },

        data() {
            return {
                // TitleComp
                smallText: 'join maxcoach at best',
                title: 'Latest Online',
                colorText: 'Courses',

                // ThreeCard
                cards: [{
                        image: 'course-02-480x298.jpg',
                        price: '$40',
                        rest: '.00',
                        description: 'Learning to Write as a Professional Author',
                        iconLesson: 'fa-regular fa-file-lines',
                        iconUser: 'fa-regular fa-user',
                        lessons: '20 Lessons',
                        students: '50 students',
                    },
                    {
                        image: 'stock-full-hd-03-480x298.jpg',
                        price: '$0',
                        rest: '.00',
                        description: 'Customer-centric Info-Tech Strategies',
                        iconLesson: 'fa-regular fa-file-lines',
                        iconUser: 'fa-regular fa-user',
                        lessons: '24 Lessons',
                        students: '769 students',
                    },
                    {
                        image: 'stock-full-hd-04-480x298.jpg',
                        price: '$19',
                        rest: '.00',
                        description: 'Open Programming Courses for Everyone: Python',
                        iconLesson: 'fa-regular fa-file-lines',
                        iconUser: 'fa-regular fa-user',
                        lessons: '17 Lessons',
                        students: '62 students',
                    }
                ],

            }
        }
    }
</script>

<style lang="scss" scoped>
    // import file.scss
    @import '../../../style/mixin.scss';
    @import '../../../style/variabili.scss';

    section {
        padding: 100px 0;
        .text-center {
            margin-bottom: 50px;
        }

        .list-circle {
            @include flex(row, center, center);
            margin-bottom: 30px;

            .small-circle:nth-of-type(1) {
                width: 10px;
                height: 10px;
                background-color: black;
            }

            .small-circle {
                width: 5px;
                height: 5px;
                border-radius: 50%;
                background-color: $color-gunSmoke;
                margin-right: 20px;
            }
        }



        .wave {
            text-align: center;
            @include center-x(50%);
            margin-top: 50px;
        }
    }
</style>