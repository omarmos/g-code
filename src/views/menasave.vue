<template>
    <v-main>
        <Header></Header>
        <v-row>
            <v-col>
        <!-- <div class="space"> -->
        <v-parallax :src="require('../assets/andreas-gucklhorn-mawU2PoJWfU-unsplash.webp')">
         <v-card-title>
            <h1>Mena Save Web & Mobile App</h1>
        </v-card-title>
        </v-parallax>

        <!-- </div> -->
            </v-col>
        </v-row>
            
        <v-container>
        <v-container>
        <v-row>
            <v-col cols="12" xl="3" lg="3" md="4" sm="12" >
                 <v-container>
                <div class="space">
                    <v-img  :src="require('../assets/icons/menasave.png')"></v-img>
                </div>
                  </v-container>
            </v-col>
            <v-col>
                <v-container>    
                <v-row>
                <div class="space">
                    <v-col>
                <h2>About Mena Save</h2> 
                    <p>
                        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quas sequi rerum optio minima consequuntur modi non corrupti magnam id repudiandae, rem odit, eligendi delectus, facere consectetur voluptas saepe quis ipsa.
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae adipisci magni error. Necessitatibus facere dolorem quibusdam qui, repellat officiis tenetur ad ipsam beatae voluptate ut pariatur, labore ducimus nobis nesciunt.
                        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quaerat sed, vitae fugiat dignissimos voluptate error sequi ipsa, asperiores neque eius officiis natus nemo ratione, vel veniam! Incidunt ipsum deserunt et!
                    </p>

                    </v-col>
                </div>
                </v-row>
                </v-container>
            </v-col>
        </v-row>
        </v-container>



         <v-container>
        <v-row>
                <div class="space">
            <v-col>
                <h2>
                    What Excel Did:
                </h2>

                <p>
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit. Adipisci, tempore saepe deleniti labore eligendi eum mollitia, doloribus fugiat nihil voluptates laudantium voluptatum qui rerum excepturi temporibus ab reiciendis nesciunt numquam!
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia, possimus. Perspiciatis omnis modi, laudantium voluptas eveniet quos ipsam cumque veniam porro dicta quisquam obcaecati distinctio nobis sed quaerat magnam similique.
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis non porro, soluta eveniet illo mollitia commodi doloribus tempore optio voluptatem, quis, architecto a sapiente cum animi qui! Officiis, quod sint!
                </p>
            </v-col>
              <v-col cols="4" class="d-none  d-md-flex d-lg-flex d-xl-flex"> 
                  <v-container>
                      
                <div class="round">

                <v-card >

                <v-img contain :src="require('../assets/jeremy-bishop-d3fZSXlJ3Ok-unsplash.jpg')" ></v-img>
                </v-card>
                </div>
                  </v-container>
            </v-col>
    </div>
        </v-row>
       
            <v-row>
                <v-col>

            <h2>
                Mr.Alameen (Mena Save CEO) said about us:
            </h2>
        <div class="space" style="background: linear-gradient(to left, rgba(192, 240, 247,0.5), rgb(12, 105, 128,0.5));">
            <v-container>
                
            <p>
                "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Incidunt minima, similique quisquam sint maiores fugit, velit repellendus at dolor nostrum laudantium laborum reiciendis sequi iure. Perferendis impedit facere deleniti ullam?"
            </p>
            </v-container>
        </div>
                </v-col>
            </v-row>
          </v-container>
          
    </v-container>
        <Footer></Footer>

    </v-main>
</template>
<script>
import Header from '../components/Header.vue'
import Footer from '../components/Footer'

export default {
    name: 'Menasave',
    components:{
        Header,
        Footer 
    }
 

}
</script>