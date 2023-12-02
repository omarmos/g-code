<template>
<v-main>
     <Header></Header>
     <Hero></Hero>
<!-- 
     <v-container>
       <v-row>
             <v-col cols="6">
         <div class="space">
           <v-card-title primary-title>            
               <h3 style="margin-top:10px;">
                  -"A website is a window through which your business says hello to the world"
                 </h3>
           </v-card-title>      
         </div>
             </v-col>
       </v-row>
     </v-container> -->
     <IconsGroup ></IconsGroup>
     <GlassCards></GlassCards>
     <PCard></PCard>
     <!-- <NewsLetterCard></NewsLetterCard> -->
      <SCards></SCards>
     <Footer></Footer>
</v-main>  


</template>


<script>

// import Animation from '../components/Animation'
import Footer from '../components/Footer.vue'
import GlassCards from '../components/GlassCards'
import IconsGroup from '../components/IconsGroup'
import Header from '../components/Header'
import Hero from '../components/Hero'
import PCard from '../components/PCard'
// import NewsLetterCard from '../components/NewsLetterCard.vue'
import SCards from '../components/SCards.vue'


export default {
  name: 'Home',
  components: {  
    // Animation,
    GlassCards,
    IconsGroup,
    Footer,
    Header,
    Hero,
    PCard,
    // NewsLetterCard,
    SCards,
  },
}
</script>