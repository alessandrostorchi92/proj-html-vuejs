<script>

export default {


    props: {

        srcImg: String,
        priceItem: String,
        descriptionItem: String,
        numberLessonsItem: String,
        numberStudentsItem: String,


    },

    methods: {

        getImagePath: function (img) {
            return new URL(`../assets/img/${img}`, import.meta.url).href;
        },
    },

}

</script>


<template>
    <div class="card-container">

        <div class="card h-100">

            <img :src="getImagePath(srcImg)" class="card-img-top" alt="Course image">

            <div class="card-body">

                <h4>{{ priceItem }}</h4>

                <p class="fs-5"><a href="#0">{{ descriptionItem }}</a></p>

                <span class="px-2"><i class="fa-regular fa-file-zipper px-1"></i>{{ numberLessonsItem }} Lessons</span>

                <span class="px-2"><i class="fa-regular fa-user px-1"></i>{{ numberStudentsItem }} Students</span>

            </div>

        </div>

    </div>
</template>



<style lang="scss" scoped>
@use "../scss/partials/_variables.scss" as *;
@use "../scss/partials/mixins";

.card-container img {
    aspect-ratio: 16/9;
}

.card {
    overflow: hidden;
    transition: transform 0.3s ease;
    transition: box-shadow 0.3s ease;

    &:hover {
    transform: scale(1.1);
    box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.5);
    }

}

.card-body h4 {
    color: $color-primary;
}

.card-body a {
    color: $color-secondary;
    text-decoration: none;
    font-weight: bold;

    &:hover {
        color: $color-primary;
    }
}

.card-body span {
    color: $color-secondary-text;
}
</style>