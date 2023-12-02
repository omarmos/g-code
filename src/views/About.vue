<template>
<div>
        <Header></Header>
        <AboutExcel/>
        <v-container>
              <v-row>
            <v-col>


                <v-card-title class="justify-center">
                     <h4>
                       The Team  
                       </h4>
                </v-card-title>
            </v-col>
        </v-row>
        </v-container>
        <Team></Team>
        <Footer></Footer>
</div>
</template>


<script>
import Header from '../components/Header.vue'
import Footer from '../components/Footer.vue'
import AboutExcel from '../components/AboutExcel.vue'
import Team from '../components/Team.vue'

export default {
    name: 'About',
    components:{
    Header,
    Footer,
        AboutExcel,
        Team,
    }

}
</script>