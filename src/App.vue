<template>
  <div id="app">

    <v-app :style="{ background: $vuetify.theme.themes[theme].background }">

      <transition name="fade">

        <router-view></router-view>
      </transition>

    </v-app>
  </div>
</template>
 
 
<script>
import '@mdi/font/css/materialdesignicons.css'


export default {
  name: 'App',
  computed: {
    theme() {
      return (this.$vuetify.theme.dark) ? 'dark' : 'light'
    }
  }
}
</script>
 