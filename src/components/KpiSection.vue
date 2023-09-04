<script>

export default {

    data() {

        return {

            columns: [

                { value: "1926", name: "FINISHED SESSIONS" },
                { value: "100%", name: "SATISFACTION RATE" },
                { value: "3092+", name: "ENROLLED LEARNERS" },
                { value: "200", name: "ONLINE INSTRUCTORS" },

            ],

        }

    },

}

</script>

<template>

    <!-- Section KPIs  -->

    <section>

        <div class="container h-100">

            <div class="row h-100 row-cols-4">

                <div class="col d-flex justify-content-center align-items-center" v-for="column in columns"
                    :key="`column.$_{i}`">

                    <div class="kpi-container text-center">
                        <div class="kpi-values fs-1 fw-semibold">{{ column.value }}</div>
                        <div class="kpi-names text-nowrap">{{ column.name }}</div>
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
    height: 300px;
    margin-top: 4rem;

    .kpi-container {
        width: 100%;
        background-image: url('../assets/img/background-pattern-grid-line-06.png');
        background-repeat: no-repeat;
        background-size: cover;
    }

    .kpi-values {
        color: $color-primary;
    }

    .kpi-names {
        color: #333333;
    }

}
</style>

