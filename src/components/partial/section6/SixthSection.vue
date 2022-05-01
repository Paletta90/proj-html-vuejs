<template>

    <section>

        <div class="text-center">
            <TitleComp :smallText="smallText" :title="title" :colorText="colorText" />
        </div>

        <ThreeCard :cards="this.cards" />

    </section>

</template>

<script>
    // Import components
    import TitleComp from '../../smallComponents/TitleComp.vue'
    import ThreeCard from '../../smallComponents/ThreeCard.vue'
    export default {

        name: 'SixthSection',

        components: {
            TitleComp,
            ThreeCard,
        },

        data(){
            return{
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

    section{
        padding: 100px 0;
    }

</style>