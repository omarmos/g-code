<template>
    <v-main>
        <Header />
        <div class="space">
            <v-row>
                <v-col>
                    <v-parallax :src="cover"></v-parallax>

                </v-col>
            </v-row>
        </div>
        <v-container>
            <v-row>
                <div class="space">
                    <v-col>


                        <h2>
                            Grow your business and establish a credible online presence.
                        </h2>
                        <p>

                            Excel is counted among the best emerging custom web development companies in Sudan. We provide a
                            wide range of website development services personalized and tailored as per the specific demands
                            of our customers. Every project needs to load fast, be pixel-perfect and user-friendly.
                            Consistency and high execution quality are based on our unique process, in which front-end is
                            coded by developers understanding the principles of UX and design.

                        </p>
                    </v-col>
                </div>
            </v-row>
        </v-container>



        <WebCards />





        <v-container>
            <v-row>
                <div class="space">
                    <v-col>
                        <p>
                            In the information age, build a website before you build a workplace. Often, your website is the
                            very first introduction that a prospective client will have to your business. When a potential
                            client arrives on your website, it takes a matter of seconds to determine whether they will stay
                            and look further, or leave and never return. Excel can make your website stand apart. Before
                            reaching out to us, take a look at the features and benefits of our website design services:
                        </p>
                    </v-col>
                </div>
            </v-row>
        </v-container>

        <!-- customer benifits -->

        <v-container>


            <div class="space" style="background-color:rgba(0,0,255,0.02);">

                <v-row>
                    <v-col>
                        <v-card-title style="word-break: normal;">
                            <h1>
                                We will ensure you:
                            </h1>
                        </v-card-title>
                        <div class="round">

                            <v-img v-tilt="{ glare: true, reverse: true }"
                                :src="require('../assets/samuel-ferrara-uOi3lg8fGl4-unsplash.jpg')" height="200px"
                                width="200px"></v-img>
                        </div>
                        <div class="round">
                            <v-img v-tilt="{ glare: true, reverse: true }"
                                :src="require('../assets/vincent-guth-62V7ntlKgL8-unsplash.jpg')" height="300px"
                                width="200px"></v-img>
                        </div>
                    </v-col>
                    <v-col>
                        <div class="round">
                            <v-card-subtitle style="size: cover;font-size: 24px; font-weight: 350">

                                <ul>
                                    <li>
                                        creating the right impression to your clients
                                        <br>
                                    </li>

                                    <li>
                                        Improve your conversion <br>
                                    </li>
                                    <li>
                                        Stay Ahead of Your Competition<br>
                                    </li>
                                    <li>
                                        Tailored to business requirement<br>
                                    </li>
                                </ul>
                            </v-card-subtitle>
                        </div>
                    </v-col>
                </v-row>
            </div>
        </v-container>
        <!-- </v-container> -->
        <v-container>
            <v-row>
                <v-col>


                    <v-container>
                        <v-row>
                            <v-col>
                                <h1>
                                    Technologies Used:
                                </h1>
                            </v-col>
                        </v-row>
                        <v-row>
                            <v-col v-for="item in items" :key="item.id">
                                <div class="space" v-tilt="{ glare: true, reverse: true }">
                                    <v-img class="icon" contain height="auto" width="auto" max-height="13em" max-width="6em"
                                        :src='item.icon'>
                                    </v-img>
                                </div>
                            </v-col>
                        </v-row>
                    </v-container>
                </v-col>
                <v-col>

                    <v-container>
                        <v-row>
                            <v-col>
                                <h1>
                                    We're experienced in building:
                                </h1>
                            </v-col>
                        </v-row>
                    </v-container>
                    <v-container>

                        <!-- </v-container> -->
                        <v-row>
                            <div class="space">
                                <v-col>
                                    <ul>
                                        <li>
                                            Point of Sale systems
                                        </li>
                                        <li>
                                            billing & invoicing systems
                                        </li>
                                        <li>
                                            Inventory software
                                        </li>
                                        <li>
                                            Business process optimisation software
                                        </li>
                                        <li>
                                            Supervisory control system
                                        </li>
                                        <li>
                                            VoIP software
                                        </li>
                                        <li>
                                            Trading software
                                        </li>
                                        <li>
                                            General ledger software
                                        </li>
                                    </ul>
                                </v-col>
                            </div>
                        </v-row>
                    </v-container>

                </v-col>
            </v-row>
        </v-container>



        <Footer />

    </v-main>
</template>
<script>
import Footer from '../components/Footer.vue'
import Header from '../components/Header.vue'
import WebCards from '../components/WebCards.vue'
export default {
    components: { WebCards, Header, Footer },
    name: 'System',
    data() {
        return {
            cover: require('../assets/christian-joudrey-u_nsiSvPEak-unsplash.jpg'),
            items: [
                {
                    id: 1,
                    icon: require('../assets/icons/HTML.svg'),
                    // color:'orange darken-2'
                },
                {
                    id: 2,
                    icon: require('../assets/icons/CSS.svg'),
                    color: 'blue-grey darken-2'
                },
                {
                    id: 3,
                    icon: require('../assets/icons/JS.svg'),
                    color: 'orange darken-2'
                },
                {
                    id: 4,
                    icon: require('../assets/icons/electronjs.svg'),
                    color: 'teal'
                },
                {
                    id: 5,
                    icon: require('../assets/icons/SASS.svg'),
                    color: 'primary'
                },
                {
                    id: 6,
                    icon: require('../assets/icons/Vue.svg'),
                    color: 'primary'
                },
                {
                    id: 7,
                    icon: require('../assets/icons/vuetifyjs.svg'),
                    color: 'primary'
                },
                {
                    id: 8,
                    icon: require('../assets/icons/bootstrap.svg'),
                    color: 'primary'
                }
            ]

        }
    },

}
</script>
<!-- <style lang="postcss">
/* List */
@import '../sass/list.sass'
</style> -->