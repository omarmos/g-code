<template>
    <v-main>
         <v-container>
  
                <v-row>

                   <v-col lg="4" md="6" sm="12" v-for="item in items" :key="item.id">
     <div class="space">
                         <v-container>
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
    name:'MobileCards',
    data() {
        return {
             items:[
          {
            id:1,
            icon: require('../assets/icons/services/013-android.svg'),
            title: "Android App Development"  ,
            p: 'According to statistics, Android OS has been installed on 66.71% of all mobile devices in the world, and this is one of the reasons why a lot of business owners prefer to have not only the iOS business solution but also the Android one. Excel Android development team created Android mobile solutions for various industries providing scalable apps that are fully integrated with the back-end software. Excel is a leading Android app development company that is highly capable of developing an app flexible enough to accommodate the needs of billions of Android users around the world.'
          },
          {
            id:2,
            icon: require('../assets/icons/services/014-apple.svg'),
             title: 'iOS App Development' ,
            p:'We at Excel build and deploy high performance, secure, and scalable iOS mobile apps that give your company the success it deserves. With our help you can make your idea reach out the world of iOS users.'
          },
          {
            id:3,
            icon: require('../assets/icons/services/015-cross-platform.svg'),
            title: 'Cross-Platform' ,
            p:' Cross-platform app development is the great way to enter market quickly on when it comes to providing mobile apps that look and feel truly native. In addition, choosing cross-platform mobile development can be more cost-effective than creating native applications separately for Android and iOS. We delight users by designing fast, secure and robust cross-platform iOS & Android apps with native performance using Flutter- whether it’s mobile, laptop, desktop, wearables, TV’s or smart displays.'
          }
             ]
        }
    },
}
</script>