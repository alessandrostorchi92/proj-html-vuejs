<script>

export default {


    props: {
    
        srcImg: String,
        priceItem: String,
        descriptionItem: String,
        numberLessonsItem: String,
        numberStudentsItem: String,
        
    
    },

}


</script>


<template>


<div class="card">

        <img class="card-img-top" :src="srcImg" alt="Course image">

        <div class="card-body">

            <h4>{{ priceItem }}</h4>

            <p>{{ descriptionItem }}</p>

            <span class="px-2"><i class="fa-regular fa-file-zipper px-1"></i>{{ numberLessonsItem }} Lessons</span>
            
            <span class="px-2"><i class="fa-regular fa-user px-1"></i>{{ numberStudentsItem }} Students</span>

        </div>

    </div>


</template>



<style lang="scss" scoped>


</style>