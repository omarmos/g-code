<template>
    <v-main>
        <Header></Header>
        <Cover></Cover>
        <v-container>
            <v-row>
                <v-col>


                    <h1>Contact Us</h1>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime asperiores illum eligendi dolorum!
                        Perspiciatis distinctio eveniet at aliquam! Repudiandae architecto facere ad aliquam ducimus fugit,
                        id necessitatibus sapiente at dolore.</p>
                </v-col>
            </v-row>
        </v-container>
        <Form></Form>
        <v-container>
            <!-- <div class="space"> -->

            <v-row>
                <v-col cols="12" lg="6" md="6" sm="12">
                    <!-- <div class="space"> -->
                    <!-- <v-card color="rgb(0,0,0,0)"> -->


                    <v-card-title>
                        <h2>Come visit us</h2>
                    </v-card-title>
                    <v-card-subtitle>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem adipisci architecto
                            cupiditate animi repellat amet, aliquam alias eligendi asperiores at aliquid blanditiis. Saepe
                            iusto natus quia iste! Eaque, corrupti quaerat!</p>
                    </v-card-subtitle>
                    <!-- </v-card> -->
                    <!-- </div> -->
                </v-col>
                <v-col cols="12" lg="6" md="6" sm="12">

                    <div class="space">

                        <iframe class="iframe"
                            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1607.3158836128332!2d32.54946522094894!3d15.558513041962913!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x168e90319775517d%3A0x1c4915b1380f2ea4!2z2YXYrNmF2Lkg2KfZhNmG2LXYsSDYp9mE2LPZg9mG2YrYjCBBZnJpY2EgU3QsIEFsIEtodXJ0dW0sIFN1ZGFu!5e0!3m2!1sen!2s!4v1612790843785!5m2!1sen!2s">
                        </iframe>
                    </div>
                </v-col>
            </v-row>
            <!-- </div> -->
        </v-container>
        <Footer></Footer>
    </v-main>
</template>
<script>
import Header from '../components/Header'
import Footer from '../components/Footer.vue'
//  import Form from '../components/Form'
import Cover from '../components/Cover'



export default {
    name: 'Contact',
    components: {
        Header,
        Footer,
        // Form,
        Cover
    }

}
</script>

