<template>
    <v-main>
      <v-lazy>

        <v-row>
            <div class="space">
            <v-col lg="6" md="6" sm="12">

            <v-card-title class="text-lg-h3 text-sm-h4 text-xs-h1">            
             
                    Subscribe to our Newsletter
                 
                    </v-card-title>
                    <v-divider></v-divider>
          <div class="space" v-tilt>

            <v-card-subtitle class="text-lg-subtitle-2 text-xs-subtitle-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquid adipisci dolorem nemo amet voluptatem? Amet ab ullam labore! Cum nihil necessitatibus animi fugiat quae magnam hic atque nam, dolores corrupti! Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus quo sunt pariatur quia tempore eum adipisci aut consequuntur rerum distinctio velit, veniam sint unde amet quas facilis corrupti culpa nisi!
            </v-card-subtitle>
            </div>
                 <!-- <form>
            <v-container> -->
                  <form>
                    <v-row>
                      <v-col cols="12">

                <v-text-field
                  v-model="email"
                  :error-messages="emailErrors"
                  label="E-mail"
                  @input="$v.email.$touch()"
                  @blur="$v.email.$touch()"
                ></v-text-field>
                      </v-col>
                      <v-spacer></v-spacer>

                      <!-- <v-col cols="3"> -->
               <div class="space">
                <v-btn
                  @click="submit"
                  color="primary"
                >
                  submit
              </v-btn>
                </div>
                      <!-- </v-col> -->
                    </v-row>
           </form>
            <!-- </v-container>
                 </form> -->


        </v-col>
            <v-col cols="6" class="d-none d-md-flex"> 
                <div class="space">

                <v-card >

                <v-img :src="require('../assets/jeremy-bishop-d3fZSXlJ3Ok-unsplash.jpg')" ></v-img>
                </v-card>
                </div>
            </v-col>
            </div>
        </v-row>

  </v-lazy>
    </v-main>
</template>
<script>
import { validationMixin } from 'vuelidate'
import {  email } from 'vuelidate/lib/validators'

export default {
  name:'NewsLetterCard',
    mixins: [validationMixin],

    validations: {
      email: { email },
       },
    data: () => ({
            // pic: require('../assets/jeremy-bishop-d3fZSXlJ3Ok-unsplash.jpg'),
            email:'',
            name:'',
            rules: [v => v.length <= 250 || 'Max 250 characters']
        }),
        computed: {
          emailErrors () {
            const errors = []
            if (!this.$v.email.$dirty) return errors
            !this.$v.email.email && errors.push('Must be a valid e-mail')
            return errors
        } 
        },
      methods: {
      submit () {
        this.$v.$touch()
      },
    },
 }
</script>