<script>

export default {

    data() {

        return {

            touchpoints: [
                { name: "382 NE 191st St # 87394 Miami, FL 33179-3899" },
                { name: "+1(305) 547-9909 (9am - 5pm EST, Monday - Friday)" },
                { name: "support@maxcoach.com" },
            ],

            socialNetworks: [
                { name: "Facebook", icon: "facebook" },
                { name: "Twitter", icon: "twitter" },
                { name: "Instagram", icon: "instagram" },
                { name: "Linkedin", icon: "linkedin" },
            ],

            linksExplore: [
                { name: "Start here" },
                { name: "Blog" },
                { name: "About us" },
                { name: "Success story" },
                { name: "Courses" },
                { name: "Contact us" },
            ],

            linksInformation: [
                { name: "Membership" },
                { name: "Purchase guide" },
                { name: "Privacy policy" },
                { name: "Terms of service" },
            ],
        };
    },

}

</script>


<template>

    <!--Footer-->

    <footer>

        <div class="bg-footer">

            <div class="container py-5">

                <div class="row">
    
                    <div class="col-6">
    
                        <h5 class="mb-3">Address</h5>
    
                        <ul class="list-unstyled" v-for="(touchpoint, i) in touchpoints" :key="`touchpoint.$_{i}`">
                            <li>{{ touchpoint.name }}</li>
                        </ul>
    
                        <div class="icons-container d-flex gap-4 py-2">
    
                            <div v-for="(social, i) in socialNetworks" :key="`social.$_{i}`">
                                <i :class="`fab fa-${social.icon}`"></i>
                            </div>
    
                        </div>
    
    
                    </div>
    
    
                    <div class="col-6">

                        <div class="footerlinks-container d-flex justify-content-end gap-5">

                            <div class="footer-explorelinks-container">

                                <h5 class="mb-3">Explore</h5>
            
                                <ul class="list-unstyled" v-for="(link, i) in linksExplore" :key="`link.$_{i}`">
                                    <li><a href="#">{{ link.name }}</a></li>
                                </ul>

                            </div>

                            <div class="footer-informationlinks-container">

                                <h5 class="mb-3">Information</h5>
            
                                <ul class="list-unstyled" v-for="(link, i) in linksInformation" :key="`link.$_{i`">
                                    <li><a href="#">{{ link.name }}</a></li>
                                </ul>

                            </div>

                        </div>

                    </div>

                    <div class="copyright-container d-flex justify-content-center align-items-center mt-5">
                        <p>© 2020 Maxcoach. All Rights Reserved</p>
                    </div>
    
                </div>

            </div>

        </div>

    </footer>

</template>


<style lang="scss" scoped>

.bg-footer {
    background-color: #171621;
    
    h5 {
        color: white;
    }

    li {
        color: #ABABAB;
    }

    a {
        color: #ABABAB;
        font-size: .9rem;
        text-decoration: none;
    }

    .footer-explorelinks-container ul li a:hover {
        color: white;
    }

    .footer-informationlinks-container ul li a:hover {
        color: white;
    }

    i {
        color: #ABABAB;
        font-size: 1.5rem;

        &:hover {
            color: white;
        }
    }

    .copyright-container {
        color: #ABABAB
    }
}

 

</style>