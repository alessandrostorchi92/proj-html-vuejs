<script>

import Navbar from './Navbar.vue';
import HeroSection from './HeroSection.vue';

export default {

    components: {

        Navbar,
        HeroSection
    }

}

</script>


<template>

    <!-- Header  -->

    <header>

        <Navbar></Navbar>
        <HeroSection></HeroSection>

    </header>

</template>


<style lang="scss" scoped>


header {
    background-image: url('../assets/img/background-pattern-wavify.png');
    width: 100%;
    height: 100%;
    object-fit: cover;
}


</style>