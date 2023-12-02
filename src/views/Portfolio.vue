<template>
   <v-app>
       <Header></Header>
       <BluryCards></BluryCards>
       <Footer></Footer>
   </v-app>
</template>

<script>
import Header from '../components/Header'
import Footer from '../components/Footer'
import BluryCards from '../components/BluryCards'

export default {
    name: 'Services',
    components: {
    Header,
    Footer,
    BluryCards
    }

}

</script>
