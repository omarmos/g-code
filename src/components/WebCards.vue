<template>
    <v-main>
         <v-container>
  
                <v-row>

                   <v-col cols="12" lg="3" md="6" sm="12" v-for="item in items" :key="item.id">
     <div class="space">
                         <v-container >
                          <!-- <div class="cards"> -->
                            <v-card color="rgba(0,0,0,0)">
                              

                     <!-- <v-icon :color="item.color"> -->
                        <v-img class="icon" contain height="auto" width="auto" max-height="7em" max-width="3em" :src='item.icon'>
                        </v-img>
                        <!-- </v-icon> -->
                     
                     <v-card-title style="word-break: normal;">
                         {{item.title}}
                     </v-card-title>
                     <v-card-subtitle style="word-break: normal;">
                         {{item.p}}
                     </v-card-subtitle>
                          <!-- </div> -->
                            </v-card>
                      </v-container>
                  
         </div>
         </v-col>
             
        </v-row>
        </v-container>
    </v-main>

</template>
<script>
export default {
    name:'WebCards',
    data() {
        return {
             items:[
          {
            id:1,
            icon: require('../assets/icons/services/001-ui-design.svg'),
            title: "Great user interface design"  ,
            p: 'At Excel we understand that a good user interface is important in the sense that it makes it easier for your target audience to clearly see what your products are. 48 percent of people cited that a website’s design is the No. 1 factor in determining a business’s credibility. It can turn potential visitors to buyers as it facilitates interactions between the user and your website or web application.'
          },
          {
            id:2,
            icon: require('../assets/icons/services/002-responsive-website.svg'),
             title: 'Mobile friendly (Responsive Design)' ,
            p:'With more than 50 percent of the internet traffic coming from mobile users, it’s imperative to provide support for users on-the-go. With responsive web design, all content and pages are flexible across all screen resolutions and devices. Whether you’re viewing a website on your smartphone or a laptop, it will be unified and easy to navigate despite the differing screen sizes. '
          },
          {
            id:3,
            icon: require('../assets/icons/services/004-hosting.svg'),
            title: 'Hosting' ,
            p:' Every website you’ve ever visited is hosted on a server. If you’re planning on creating an online presence, reliable web hosting is essential. At Excel we find the best Hosting Solutions for your business needs. Choosing the right hosting plan will mean having access to the right allocation of resources to keep your website loading quickly and reliably for your visitors,'
          },
          {
            id:4,
            icon: require('../assets/icons/services/003-email.svg'),
            title: 'Professional email' ,
            p:'Maintain a Professional image with a Custom Domain-based email. Excel provides Professional Email Solutions to help your business maintain a professional image. Keeping your customer’s trust and appearing credible online.'
          }
             ]
        }
    },
}
</script>