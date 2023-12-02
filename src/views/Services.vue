
<template>
  <v-main>
       <Header></Header>
       <Cover></Cover>
         <v-divider></v-divider>
             <v-container>
       <!-- <div class="space"> -->
      <v-row >
        <v-col>
         
           <v-card-title  primary>
              <h1>
                  Our Services
              </h1> 
            </v-card-title>
          <div class="space" v-tilt>


            <v-card-subtitle>Excel is counted among the best emerging custom web development companies in Sudan. We provide a wide range of website development services personalized and tailored as per the specific demands of our customers. Every project needs to load fast, be pixel-perfect and user-friendly. Consistency and high execution quality are based on our unique process, in which front-end is coded by developers understanding the principles of UX and design.</v-card-subtitle>
            </div>
        </v-col>
       </v-row>
     </v-container>
       <SCards></SCards>
         <v-divider></v-divider>
       <Footer></Footer>
  </v-main>  
</template>


<script>

import Cover from '../components/Cover'
import SCards from '../components/SCards'
import Header from '../components/Header'
import Footer from '../components/Footer'


export default {
  name: 'Portfolio',
  components: {  
    Cover,
    SCards,
    Header,
    Footer
    
  },
}
</script>