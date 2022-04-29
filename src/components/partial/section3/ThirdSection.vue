<template>

    <section>
        
        <div class="text-center">
            <TitleComp :smallText="smallText" :title="title" :colorText="colorText"/>
        </div>

        <ThreeCard :cards="this.cards"/>

        
    </section>

</template>

<script>
    // Import components
    import TitleComp from '../../smallComponents/TitleComp.vue'
    import ThreeCard from './ThreeCard.vue'

    export default {
        name: 'ThirdSection',

        components:{
            TitleComp,
            ThreeCard,
        },

        data(){
            return{
                // TitleComp
                smallText: 'join maxcoach at best',
                title: 'Latest Online',
                colorText: 'Courses',

                // ThreeCard
                cards:[
                    {
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

    section {
        padding: 100px 0;

        .text-center{
            margin-bottom: 50px;
        }
    }

</style>