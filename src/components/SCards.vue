<template>
  <v-main>
    <v-main v-for="item in items" :key="item.id">
        <v-container>
            
        <v-row>
            <v-col>

                <v-card-title >
                     <h1>
                        {{item.title}}
                       </h1>
                </v-card-title>
            </v-col>
        </v-row>
        </v-container>


        <v-container >
             <div class="space" style="background: linear-gradient(to left, rgba(192, 240, 247,0.5), rgba(12, 105, 128,0.5));">
         <v-container >


                <!-- <v-card-subtitle> --> <p>
                  {{item.subtitle}}
                      <v-btn x-small color="secondary" :to="item.to" > read more</v-btn>
                  </p>
         </v-container>


                    <!-- </v-card-subtitle> -->
         </div>
        </v-container>
    </v-main>

  </v-main>
</template>
<script>
export default {
  name:'SCard',
    data() {
      return {
        items:[
          {
            id:1,
            title: 'Web Development',
            subtitle:'o Excel is counted among the best emerging custom web development companies in Sudan. We provide a wide range of website development services personalized and tailored as per the specific demands of our customers. Every project needs to load fast, be pixel-perfect and user-friendly. Consistency and high execution quality are based on our unique process, in which front-end is coded by developers understanding the principles of UX and design.',
            to: '/web-development'
          },
          {
            id:2,
            title: 'Mobile Development',
            subtitle:' Excel is counted among the best emerging custom web development companies in Sudan. We provide a wide range of website development services personalized and tailored as per the specific demands of our customers. Every project needs to load fast, be pixel-perfect and user-friendly. Consistency and high execution quality are based on our unique process, in which front-end is coded by developers understanding the principles of UX and design.',
            to: '/mobile-development'
          },
         {
            id:3,
            title: 'System Development',
            subtitle:'o Excel is counted among the best emerging custom web development companies in Sudan. We provide a wide range of website development services personalized and tailored as per the specific demands of our customers. Every project needs to load fast, be pixel-perfect and user-friendly. Consistency and high execution quality are based on our unique process, in which front-end is coded by developers understanding the principles of UX and design.',
            to: '/system-development'
          },
           {
            id:4,
            title: 'Digitial marketing',
            subtitle:' Excel is counted among the best emerging custom web development companies in Sudan. We provide a wide range of website development services personalized and tailored as per the specific demands of our customers. Every project needs to load fast, be pixel-perfect and user-friendly. Consistency and high execution quality are based on our unique process, in which front-end is coded by developers understanding the principles of UX and design.',
            to: '/digital-marketing'
          }
        ],
        }
    },
}
</script>
<style lang="css">
.divs {
    display: table-cell;
}
  
</style>