<template background-color="primary">
<v-content >
<!-- <div class="space" > -->
         <v-card-title class="ma-15 justify-center" primary-title>
             <h4>
                 OUR SERVICES
             </h4>
         </v-card-title>  
    <v-row>
        <v-col lg="3" md="6" sm="12"   v-for="item in items" :key="item.id">

    <div class="container">

        <div class="card" v-tilt="{glare:true, reverse: true }">
            <div class="content">
             
                <!-- <h2> -->
                     <v-img class="icon h2"
                            contain
                            height="auto"
                            width="auto"
                            max-height="6.5em"
                            max-width="2em"
                            :src='item.title'
                            style="fill:linear-gradient(to bottom, rgba(192, 240, 247,0.5), rgb(12, 105, 128,0.5));"
                            >
                     </v-img>
                    <!-- <v-icon> -->
                    <!-- {{ item.title }} -->
                    <!-- </v-icon> -->
                    <!-- </h2> -->
                <v-card-title>
                <h3>{{item.subtitle}}</h3>
                </v-card-title>
                <v-card-subtitle>

                <p>{{ item.description }}.</p>
                </v-card-subtitle>
                <router-link :to="item.to" class="a" >read more </router-link>
                    <!-- <a :href="item.to">read more</a> -->
                   
            </div>
        </div>
    </div>
    </v-col>
    </v-row>
<!-- </div> -->
        
</v-content>        
    
</template>
<script>
export default {
    name: 'GlassCards',
    data() {
        return {
            items:[
                {
                    id:1,
                    title: require('../assets/icons/web.svg'),
                    subtitle: 'Web Development',
                    to:'/web-development',
                    description: 'Creative web design and development, offering solutions in both large, complex web applications, and smaller informative landing pages.'
                },
                {
                    id:2,
                    title: require('../assets/icons/MobileD.svg'),
                    subtitle: 'Mobile Development',
                    to:'/mobile-development',
                    description: 'Immersive mobile app solutions, well-structured iOS and Android app development that transforms businesses and deliver great customer experience.'
                },
                {
                    id:3,
                    title: require('../assets/icons/system.svg'),
                    subtitle: 'System Development',
                    to:'/system-development',
                    description: 'Our software product development services ensure high product functionality that results much easier product and exceptional user experience'
                },
                {
                    id:4,
                    title: require('../assets/icons/Dmarketing.svg'),
                    subtitle: 'Digital Marketing',
                    to:'/digital-marketing',
                    description: 'Effective digital marketing campaigns that drive leads and boost sales. We help design and implement digital marketing campaigns that generate leads that convert to sales that make you stand apart from your competitors and steal the spotlight.'
                }
            ]
        }
    },
}
    
    
</script>
