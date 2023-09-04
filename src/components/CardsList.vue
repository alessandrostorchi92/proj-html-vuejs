<script>

import SingleCard from './SingleCard.vue';

export default {

    components: {

        SingleCard

    },

    data() {

        return {

            courses: [

                {
                    img: "motivation-course-06-480x298.jpg",
                    price: "$30.00",
                    description: "How to be Successful: Create A Growth Mindset For Success",
                    numberLessons: "3",
                    numberStudents: "50",
                },

                {
                    img: "motivation-course-05-480x298.jpg",
                    price: "$30.00",
                    description: "How to Build Confidence in Your Abilities",
                    numberLessons: "1",
                    numberStudents: "50",
                },

                {
                    img: "motivation-course-04-480x298.jpg",
                    price: "$20.00",
                    description: "Productivity Machine – Focus in a Distracted World",
                    numberLessons: "5",
                    numberStudents: "50",
                },

                {
                    img: "motivation-course-03-480x298.jpg",
                    price: "$20.00",
                    description: "Effective Time Management Mastery – Complete Guide",
                    numberLessons: "18",
                    numberStudents: "50",
                },

                {
                    img: "motivation-course-02-480x298.jpg",
                    price: "$25.99",
                    description: "Body Language Secrets for Entrepreneurs",
                    numberLessons: "19",
                    numberStudents: "50",
                },

                {
                    img: "motivation-course-01-480x298.jpg",
                    price: "$19.99",
                    description: "Management Skills: The Science of Leadership",
                    numberLessons: "17",
                    numberStudents: "50",
                },

            ],
        }
    }

}

</script>


<template>

    <section>

        <!-- Cardslist Section  -->

        <div class="titles-container text-center mt-5 py-5">

            <div class="title-section mb-4">BEGIN YOUR JOURNEY AT MAXCOACH</div>

            <h2 class="subtitle-section fs-1">Latest <span class="green-text">Online Courses</span></h2>

        </div>

        <div class="container">

            <div class="row row-cols-3 g-4">

                <SingleCard v-for="(course, i) in courses" :key="`course_${i}`" :srcImg="course.img" :priceItem="course.price" :descriptionItem="course.description" :numberLessonsItem="course.numberLessons" :numberStudentsItem="course. numberStudents"></SingleCard>

            </div>

        </div>


    </section>

</template>



<style lang="scss" scoped>
@use "../scss/partials/_variables.scss" as *;
@use "../scss/partials/mixins";


.title-section {
    color: $color-secondary-text;
}

.green-text {
    color: $color-primary;
}
</style>