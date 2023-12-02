<template>
  <div class="space">

    <v-main>
      <v-row>
        <v-col>
          <v-app-bar flat class=" m-6" color="rgb(255, 255, 255, 0.02)">
            <v-app-bar-title>
              <v-tab to="/">
                <v-img :src=svg height="30px" width="50px"></v-img>
              </v-tab>
            </v-app-bar-title>
            <v-spacer></v-spacer>

            <!-- <v-avatar
          :color="$vuetify.breakpoint.smAndDown ? 'grey darken-1' : 'transparent'"
          size="32"
        ></v-avatar> -->
            <v-content>
              <v-tab centered class="hidden-md-and-down" to="/">Home </v-tab>

            </v-content>
            <v-content>
              <v-tab centered class="hidden-md-and-down" to="/portfolio">Portfolio </v-tab>

            </v-content>
            <v-content>
              <v-tab centered class="hidden-md-and-down" to="/aboutus"> About </v-tab>

            </v-content>
            <v-content>
              <v-tab centered class="hidden-md-and-down" to="/contact">Contact</v-tab>

            </v-content>
            <!-- <v-content>
              <v-menu offset-y>
                <template v-slot:activator="{ on, attrs }">
                  <v-tab centered class="hidden-md-and-down" v-bind="attrs" v-on="on">
                    Services
                  </v-tab>
                </template>

                <div class="space">
                  <v-list color="rgb(0,139,139, 0.5)">
                    <v-list-item v-for="(item, index) in items" :key="index" :to="item.to">
                      <v-list-item-title to='/ourservices'>{{ item.title }}</v-list-item-title>
                    </v-list-item>
                  </v-list>
                </div>
              </v-menu>
            </v-content> -->
            <!-- <v-content>
         <v-tab centered class="hidden-md-and-down"  to="/ourservices">Services </v-tab>
            class="ml-n9"
         </v-content> -->


            <v-spacer></v-spacer>
            <v-btn to="/nav" class="hidden-lg-only" icon><v-icon>menu</v-icon></v-btn>
            <v-btn @click="toggleTheme()" icon><v-img :src="('/src/assets/dark_mode-black-18dp.svg')"></v-img></v-btn>
            <v-switch onclick="toggleTheme()"></v-switch>


          </v-app-bar>

        </v-col>
      </v-row>
    </v-main>
  </div>
</template>
  
<script>
export default {
  name: 'Header',
  data() {
    return {
      items: [
        {
          title: 'Web Development',
          to: '/ourservices'
        },
        {
          title: 'Mobile Development',
          to: '/ourservices'
        },
        {
          title: 'Digital Marketing',
          to: '/ourservices'
        },
        {
          title: 'System Development',
          to: '/system-development'
        },
      ],
      svg: ('/src/assets/xl-sada/3.png')
    }
  },
  methods: {
    toggleTheme() {
      this.$vuetify.theme.dark = !this.$vuetify.theme.dark;


    }
  }
}
</script>
  