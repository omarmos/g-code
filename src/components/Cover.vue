<template>
 <v-main>
   <div class="space">

  <v-row>
    <v-col>

      <v-parallax  :src="require('../assets/andreas-gucklhorn-mawU2PoJWfU-unsplash.webp')"></v-parallax>
<!--       
  <div class="space">
    <div class="parent">
      <div class="child">
        <h2 class="hidden-md-and-down"> Frosted Glass Effect </h2>
        <h4 class="ml-10 mt-3 hidden-sm-and-up" style="font-size: 0.7em"> small Responsive glass effect</h4>
        <h4 class="ml-15 pl-5 mt-8 hidden-lg-only hidden-xs-only" style="font-size: 0.9em" > mid Responsive glass effect</h4>
        </div>
    </div>
          -->
  <!-- </div> -->  
  
      </v-col>
    </v-row>
   </div>
</v-main>    
</template>
<script>
export default {
  name: 'Cover',
}
    
    
</script>
<style lang="css">
@import '../sass/cover.css';
</style>