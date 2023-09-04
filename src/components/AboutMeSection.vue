<script>

export default {

}

</script>


<template>

    <!-- Section About me  -->

    <section>

        <!-- First Section  -->

        <div class="container">

            <div class=" title-section mb-4">ABOUT ME</div>

        </div>

        <div class="container">

            <div class="row">

                <div class="col-6">

                    <h2 class="fs-1">How to Be an Alpha <br> Male: The 15 Habits of <br> True Alphas</h2>

                </div>

                <div class="col-6">

                    <p class="fw-semibold">Want to learn how to be <span class="green-text">an alpha male</span>? How to be more masculine? <br> How to be the man you’ve always wanted to be?</p>

                    <p class="specs-text fw-light">Your goal is to show the consistency of business, core values, and customer care. <br> Punctuality, responsibility, individuality, accuracy, enthusiasm – you have to clearly <br> explain how these qualities are applicable to your work. And the important thing i<br>you do love what you do.</p>

                </div>

            </div>

        </div>

        <!-- Second Section  -->

        <div class="container mt-5 py-5">

            <div class="row">

                <div class="col-6">

                    <div class="cover-video position-relative">

                        <img src="../assets/img/home-movation-video-poster-670x450.jpg" alt="Cover Video">
                        <a href="#"><img src="../assets/img/icon-youtube-play.png" alt="Youtube Icon" class="youtube-icon"></a>

                    </div>

                </div>

                <div class="col-6 d-flex justify-content-center align-items-center">

                    <div class="desc-container ms-5 px-5">

                        <p class="fs-3 fw-light">"Every morning you have two choices: continue to sleep with your dreams, or wake up and chase them."</p>
    
                        <img src="../assets/img/home-movation-shape-01.png" alt="">
    
                        <div class="fs-4 fw-fw-medium mt-3">Kaixa Stark</div>
    
                        <div class="mt-2"><small>WINGMAN</small></div>

                    </div>



                </div>

            </div>


        </div>


    </section>

</template>


<style lang="scss" scoped>
@use "../scss/partials/_variables.scss" as *;
@use "../scss/partials/mixins";

section {
    margin-top: 4rem;

    .title-section {
        color: $color-primary;
    }

    .green-text {
        color: $color-primary;
    }

    .specs-text {
        color: $color-secondary-text;
    }

    .youtube-icon {
        @include mixins.absolute-center;
    }

    .desc-container p {
        color: $color-primary-text;
    }

    .desc-container small {
        font-size: 14px;
        color: $color-secondary-text;
    }

}</style>