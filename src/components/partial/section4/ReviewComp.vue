<template>

    <div id="contenitore">

        <!-- Prima recensione opaca -->
        <div class="firstReview">

            <p class="textBold">The MaxCoach team works really hard to ensure high level of quality</p>

            <p class="paragraph">I am happy with their arrangement of lessons and subjects. They</p>

        </div>

        <!-- Seconda recensione -->
        <div class="secondReview">

            <p class="textBold">Professional team of specialists and passionate mentors at reach</p>

            <p class="paragraph">I need to get a certification for English proficiency and MaxCoach is my best choice.
                Their tutors are smart and professional when dealing with students</p>

            <!-- User -->
            <div class="user">

                <!-- img user -->
                <div class="imgUser">
                    <img src="../../../assets/image/testimonial-avata-01.jpg" alt="" width="100%">
                </div>

                <!-- Dati user -->
                <div>
                    <p class="textBold">MADLEY PONDOR</p>
                    <p class="paragraph">/ IT Specialist</p>
                </div>

            </div>

        </div>

        <!-- Terza recensione opaca -->
        <div class="thirdReview">

            <!-- User -->
            <div class="user">

                <!-- img user -->
                <div class="imgUser">
                    <img src="../../../assets/image/testimonial-avata-02.jpg" alt="" width="100%">
                </div>

                <!-- Dati user -->
                <div>
                    <p class="textBold">MINA HOLLACE</p>
                    <p class="paragraph">/ Freelancer</p>
                </div>

            </div>

        </div>

    </div>

</template>

<script>
    export default {
        name: 'ReviewComp'
    }
</script>


<style lang="scss" scoped>
    // import file.scss
    @import '../../../style/mixin.scss';
    @import '../../../style/variabili.scss';

    #contenitore {
        width: calc(60% - 50px);
        margin-left: 50px;

        .textBold {
            margin-bottom: 10px;
        }

        .firstReview, 
        .thirdReview{
            @include center-x(80%);
            box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);;
            opacity: 0.5;
        }

        .firstReview {
            padding: 15px 15px 0px 15px;
            border-top-left-radius: 20px;
            border-top-right-radius: 20px;
        }

        .secondReview {
            box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
            padding: 15px 15px;
            border-radius: 20px;
            

            .paragraph{
                margin-bottom: 10px
            }
        }

        .user {
            @include flex(row, initial, center);

            .imgUser {
                width: 60px;
                height: 60px;
                margin-right: 15px;

                img {
                    border-radius: 50%;
                }
            }

        }

        .thirdReview{
            border-bottom-left-radius: 20px;
            border-bottom-right-radius: 20px;
            padding: 0px 15px 15px 15px;
        }

    }
</style>