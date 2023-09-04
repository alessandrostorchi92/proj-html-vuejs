<script>

export default {

    data() {

        return {

            navLinks: [

                { name: "Home" },
                { name: "Pages" },
                { name: "Courses" },
                { name: "Features" },
                { name: "Blog" },
                { name: "Shop" },

            ],

            socialNetworks: [

                { name: "Twitter", icon: "twitter" },
                { name: "Facebook", icon: "facebook" },
                { name: "Instagram", icon: "instagram" },
                { name: "Linkedin", icon: "linkedin" },

            ],

        }
    }

}

</script>


<template>

    <!-- Navbar  -->

    <nav>

        <div id="navbar-container">

            <!-- Left side navbar  -->

            <div class="logo-container">

                <img src="../assets/img/dark-logo.png" alt="Logo Max Coach">

            </div>

            <!-- Central side navbar  -->

            <div class="menulist-container d-flex gap-4">

                <li class="nav-item dropdown" v-for="(link, i) in navLinks" :key="`link.$_{i}`">

                    <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown"
                        aria-expanded="false">{{ link.name }}</a>

                    <ul class="dropdown-menu">
                        <li><a class="dropdown-item" href="#">Action</a></li>
                        <li><a class="dropdown-item" href="#">Another action</a></li>
                        <li><a class="dropdown-item" href="#">Something else</a></li>
                    </ul>

                </li>

            </div>

            <!-- Right side navbar  -->

            <div class="icons-container d-flex gap-4">

                <div v-for="(social, i) in socialNetworks" :key="`social.$_{i}`">
                    <i :class="`fab fa-${social.icon}`"></i>
                </div>

            </div>

        </div>

    </nav>
</template>

<style lang="scss" scoped>

@use "../scss/partials/_variables.scss" as *;
@use "../scss/partials/mixins";

#navbar-container {
    @include mixins.flex-content;
    justify-content: space-around;
    height: 80px;

    img {
        width: 180px;
    }

    ul {
        list-style: none;
    }

    li {
        display: inline-block;
    }

    .nav-link {
        color: $color-secondary;

        &:hover {
            color: $color-primary;
            text-decoration: underline;
            text-decoration-color: $color-primary;
        }
    }

    i {
        font-size: 1.2rem;
        color: #333333;

        &:hover {
            color: $color-primary;
        }
    }

    .dropdown-item:hover {
        color: $color-primary;
        background-color: transparent;
    }

}

</style>