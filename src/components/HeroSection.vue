<script>

export default {

}

</script>

<template>

    <!-- Hero Section -->

    <div class="hero-section-container">

        <div class="row justify-content-center align-items-center">

            <!-- Left side hero section  -->

            <div class="col-6 left-side">

                <div class="mb-4">I'M WINGMAN</div>

                <h1 class="mb-4 fs-1">Peace On Earth A <br> Wonderful Wish <br> But No Way</h1>

                <p class="mb-4">Success isn't overnight.It's when everyday you get a little <br> better than the day before.It's all adds up.</p>

                <div>
                    <button type="button" class="py-3">Get Started For Free <i class="fa-solid fa-arrow-right-long ms-3"></i></button>
                </div>

            </div>

            <!-- Right side hero section  -->

            <div class="col-6 right-side">

                <img src="../assets/img/home-movation-hero-image.png" alt="Wingman image">

            </div>

        </div>

    </div>

</template>


<style lang="scss" scoped>
@use "../scss/partials/_variables.scss" as *;
@use "../scss/partials/mixins";

.left-side {
    padding-left: 6.4rem;

    p {
        color:#696969;
    }
}

.right-side {
    display: flex;
    justify-content: center;
    background-image: url('../assets/img/home-movation-shape-face-300x267.png');
    background-repeat: no-repeat;
    background-position: bottom 50px right 100px;
    background-size: 360px;
}

img {
    width: 400px;
}

button {
    font-size: 0.9rem;
    width: 260px;
    background-color: $color-primary;
    border: none;
    color: white;
    font-weight: bold;

    &:hover {
        background-color: $color-secondary;
    }

}

</style>