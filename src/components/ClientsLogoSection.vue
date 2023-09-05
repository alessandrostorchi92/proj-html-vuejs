<script>

export default {

    data() {

        return {

            logosImg: [

                { img: "client-logo-05-primary.png" },

                { img: "client-logo-06-primary.png" },

                { img: "client-logo-07-primary.png" },

                { img: "client-logo-04-primary.png" },

                { img: "client-logo-03-primary.png" },

                { img: "client-logo-02-primary.png" }

            ]

        }
    },

    methods: {

        getImagePath: function (img) {
            return new URL(`../assets/img/${img}`, import.meta.url).href;
        }
    },

}

</script>



<template>

    <div class="container py-5">

        <div class="row row-cols-6 g-5">

            <div class="logo-container d-flex justify-content-center align-items-center" v-for="(logo, i) in logosImg" :key="`logo_${i}`">
            
            <img :src="getImagePath(logo.img)" alt="Logo image">
            
            </div>

        </div>

    </div>

</template>



<style lang="scss" scoped>


</style>

