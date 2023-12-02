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


                        <p>
                            Excel produces top-notch customisable stand-alone Desktop system development services. We ensure
                            high product functionality regardless of its complexity. Delivering a much easier product and an
                            exceptional user experience. Our expertise is exhibited in our systems; where computationally
                            expensive processes, state-of-art graphics, computer vision capabilities ,top performance,
                            utility of hardware access and well founded security are achieved.
                        </p>
                    </v-col>
                </div>
            </v-row>
        </v-container>



        <SystemCards />





        <v-container>
            <v-row>
                <div class="space">
                    <v-col>
                        <p>Upgrading to having your own business stand-alone system will give you the privilege of
                            automation of the organisation's tasks as well as reporting the progress or lags in the
                            organisation's activities. This improves company's efficiency and effectiveness of the company's
                            activities. The software reduces the workload and automation of activities.</p>
                    </v-col>
                </div>
            </v-row>

            <!-- customer benifits -->

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
                            <v-card-subtitle style="font-size: 24px; font-weight: 350">

                                <ul>
                                    <li>
                                        Cut cost by automating routine tasks <br>
                                    </li>

                                    <li>
                                        Improve the efficiency of staff<br>
                                    </li>
                                    <li>
                                        Measure and increase office productivity<br>
                                    </li>
                                    <li>
                                        Streamline business operations and accounts<br>
                                    </li>
                                    <li>
                                        Replace paper processes<br>
                                    </li>
                                    <li>
                                        Communicate more efficiently with customers, suppliers and partners.<br>
                                    </li>
                                </ul>
                            </v-card-subtitle>
                        </div>
                    </v-col>
                </v-row>
            </div>
        </v-container>
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
import SCards from '../components/SCards.vue'
// import nodejs from '../assets/icons/nodejs.svg'

export default {
    components: { SCards, Header, Footer },
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
@import 'src/sass/list.sass'
</style> -->