<template>
<v-main>
	<v-row>
		<v-col> 
			<div class="space">
               <v-carousel :show-arrows="false" >
                 <v-carousel-item
                   v-for="(item,i) in items"
                   :key="i"
                   :src="item.src"
                 ></v-carousel-item>
               </v-carousel>
           </div>
	</v-col>
  </v-row>
</v-main>
  
</template>

	

   
<script>
export default {
    name: 'Animation' ,
    data() {
		return {
			items: [
          {
            src: require( '../assets/andreas-gucklhorn-mawU2PoJWfU-unsplash.webp'),
          },
          {
            src: require('../assets/christian-joudrey-u_nsiSvPEak-unsplash.jpg'),
          },
          {
            src :require( '../assets/jonatan-pie-3l3RwQdHRHg-unsplash.jpg'),
          },
          {
            src: require( '../assets/johannes-plenio-hvrpOmuMrAI-unsplash.jpg'),
          },
        ],
		}
	},
}
</script>
  <!--   <script src="../js/demo.js"></script>
		<script src="../js/imagesloaded.pkgd.min.js"></script>
		<script src="../js/anime.min.js"></script>
		<script src="../js/demo6.js"></script>
		
		<style lang="css">
		@import '/src/scss/base'	
		</style> -->