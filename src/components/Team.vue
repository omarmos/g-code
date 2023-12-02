<template>
    <v-main>
        <v-row>
            <v-col cols="12" lg="6" md="12" sm="12" v-for="item in items" :key="item.id">
                <div class="space">
                <v-img height="30em" class="white--text  align-end" :src="item.src">
                    <v-card-title  primary-title>
                            <h1>
                            {{ item.title }}
                            </h1>
                        </v-card-title>
                        <v-card-subtitle>
                            
                            {{ item.subtitle }}
                        </v-card-subtitle>
                </v-img>
                    </div> 
                    <!-- <div class="space"> -->
                        
                    <!-- </div> -->

            </v-col>
        </v-row>
    </v-main>
</template>
<script>
export default {
    name:'Team',
    data() {
        return {
            items:[
                {
                    id:1,
                    src: require('../assets/approachable-professional-headshot_1.jpg'),
                    title: 'Ahmed Behairi',
                    subtitle:'CEO'
                },
                {
                    id:3,
                    src: require('../assets/Professional-Headshot-and-Corporate-Photo-1.jpg'),
                    title: 'The Awseome Fishlegs ',
                    subtitle:'CEO'
                }
            ]
        }
    },
}
</script>