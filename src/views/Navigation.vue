<template>
   <v-main>
       <div class="navigation">
           <div class="navArea" >
               <ul>
                   <li>
                       <v-tab text to="/" @mouseenter='image=require(`../assets/1216690.webp`)'>Home</v-tab>
                   </li>
                   <v-divider></v-divider>
                   <li>
                       <v-tab text to="/portfolio" @mouseenter='image=require(`../assets/Professional-Headshot-and-Corporate-Photo-1.jpg`)'>Portfolio</v-tab>
                   </li>
                   <v-divider></v-divider>
                    <li>
                       <v-tab text to="/aboutus" @mouseenter='image=require(`../assets/Professional-Headshot-and-Corporate-Photo-1.jpg`)'>About Us</v-tab>
                   </li>
                   <v-divider></v-divider>
                   <li>
                       <v-tab text to="/ourservices" @mouseenter='image=require(`../assets/denys-nevozhai-2vmT5_FeMck-unsplash.jpg`)'>Our Services</v-tab>
                   </li>
                   <v-divider></v-divider>
                   <li>
                       <v-tab text to="/contact" @mouseenter='image=require(`../assets/christian-joudrey-u_nsiSvPEak-unsplash.jpg`)'>Contact Us</v-tab>
                   </li>
                </ul>
           </div>
            <div class="imgArea" >
                    <v-img id="slider" :src='image' ></v-img>
                </div>
       </div>

   </v-main>
</template>
<script>
export default {
    name:'Navigation',
        data() {
            return {
                image: null            }
        },
}
</script>
<style lang="css">
@import '../sass/nav.css'

</style>