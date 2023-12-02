<template>
<v-main>
  <v-card-title class="ma-10" primary-title>
   <h4>OUR CLIENTS</h4>
  </v-card-title>

<v-container>
  <v-row justify="space-around">
      <v-col v-for="item in items" :key="item.id">
    <div class="round" v-tilt="{ glare:true }">

    <v-icon
    class="icon"
      large
      :color="item.color"
    >
     {{item.icon}}
    </v-icon>
</div>

      </v-col>
  </v-row>
  
    
</v-container>
  </v-main>
</template>
<script>
export default {
    name:'IconsGroup',
    data() {
      return {
        items:[
          {
            id:1,
            icon: 'mdi-domain',
            color:'orange darken-2'
          },
          {
            id:2,
            icon: 'mdi-message-text',
            color:'blue-grey darken-2'
          },
          {
            id:3,
            icon: 'mdi-arrow-up-bold-box-outline',
            color:'orange darken-2'
          },
          {
            id:4,
            icon: 'mdi-email',
            color:'teal'
          },
          {
            id:5,
            icon: 'mdi-dialpad',
            color:'primary'
          }
        ]
      }
    },
}
</script>

<style lang="scss">
.icon {
    margin:10px;
    padding: 30px
}
//  h1:after {
//       content: "";
//       background: black;
//       $material-dark: (
//         background: white,
//       );
//       width: 60px;
//       height: 1px;
//       position: absolute;
//       bottom: 0%;
//       left: 50%;
//       transform: translateX(-50%);

//       @media only screen and (max-width: 599px) {
//         width: 30px;
//       }
//     }  
</style>
