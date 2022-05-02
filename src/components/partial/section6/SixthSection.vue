<template>

    <section>

        <div class="center">
            <div class="text-center">
                <ParagraphComp :smallText="smallText" :title="title" :colorText="colorText" />
            </div>

            <ThreeCard :cards="this.cards" />
        </div>


    </section>

</template>

<script>
    // Import components
    import ParagraphComp from '../../smallComponents/ParagraphComp.vue'
    import ThreeCard from '../../smallComponents/ThreeCard.vue'
    export default {

        name: 'SixthSection',

        components: {
            ParagraphComp,
            ThreeCard,
        },

        data() {
            return {
                // TitleComp
                smallText: 'read for more joyment',
                title: 'Latest from',
                colorText: 'Our Blogs',

                // three card
                cards: [{
                        image: 'artist-blog-03-480x325.jpeg',
                        type: 'blog',
                        price: 'Artist',
                        rest: '',
                        description: 'Brush Strokes Energize Trees in Paintings',
                        iconLesson: 'fa-regular fa-calendar',
                        iconUser: 'fa-regular fa-user',
                        lessons: 'May 15, 2020',
                        students: '688 views',
                    },
                    {
                        image: 'artist-blog-01-480x325.jpg',
                        type: 'blog',
                        price: 'Artist',
                        rest: '',
                        description: 'Pocket-Sized Notebooks Hold Miniature Paintings',
                        iconLesson: 'fa-regular fa-calendar',
                        iconUser: 'fa-regular fa-eye',
                        lessons: 'May 15, 2020',
                        students: '603 views',
                    },
                    {
                        image: 'artist-blog-02-480x325.jpg',
                        type: 'blog',
                        price: 'Artist',
                        rest: '',
                        description: 'Connection Between Self-Portraits and Identity',
                        iconLesson: 'fa-regular fa-calender',
                        iconUser: 'fa-regular fa-eye',
                        lessons: 'May 15,2020',
                        students: '397 views',
                    }
                ],
            }
        }
    }
</script>

<style lang="scss" scoped>
    @import '../../../style/mixin.scss';

    section {
        background-color: #f9f9f9;
        margin: 50px 0;
        padding: 100px 0;

        .center{
            @include center-x(60%)
        }
    }
</style>