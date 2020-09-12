<template>
<div class="contact">
   
   <v-container grid-list-md >
    <v-layout row wrap>
  <v-flex xs12 sm5 >
  
  <p>Get in touch with EBBS(Education Builds the Basis of Society) to learn more about our work and how you can get involved</p>

          <v-text-field
            v-model="last"
            label="Name*"
            
          ></v-text-field>
        
        
          <v-text-field
            v-model="last"
            label="E-Mail*"
            
          ></v-text-field>
        
         <v-textarea
          name="input-7-1"
          label="Message"
          value=""
          hint="Hint text"
        ></v-textarea>
          
         <v-btn @click="submit">submit</v-btn> 
           
        <v-card>
          <p>Subscribe to get latest updates!</p>
          <v-text-field
            v-model="email"
            :rules="[rules.required, rules.email]"
            label="E-mail*"
            >
          </v-text-field>
          <v-flex xs12>
          <v-btn block @click="submit">Subscribe Now</v-btn> </v-flex>
        </v-card>
     
</v-flex>
<v-flex xs 12 sm2><v-spacer></v-spacer></v-flex>
<v-flex xs12 sm5>
        <v-card>

         <h2>Address Info.</h2>
         <p>EBBS - Education Builds The Bases of Society</p>
           <v-flex xs>
             
            <base-subheading>Contact</base-subheading>
            <v-list class="transparent">
              <v-list-tile>
                <v-list-tile-avatar
                  color="light-blue"
                >
                  <v-icon
                    
                    dark
                  >
                    mdi-email-outline
                  </v-icon>
                </v-list-tile-avatar>
                <v-list-tile-title >EMAIL</v-list-tile-title>
                <v-list-tile-sub-title >
                  ebbspak@outlook.com
                </v-list-tile-sub-title>
              </v-list-tile>
              <v-list-tile>
                <v-list-tile-avatar
                  color="light-blue"
                >
                  <v-icon
                    
                    dark
                  >
                    mdi-map-marker
                  </v-icon>
                </v-list-tile-avatar>
                <v-list-tile-title>Location</v-list-tile-title>
                <v-list-tile-sub-title>
                  Karachi,Pakistan
                </v-list-tile-sub-title>
              </v-list-tile>
              <v-list-tile>
                <v-list-tile-avatar
                  color="light-blue"
                >
                  <v-icon
                   
                    dark
                  >
                    mdi-phone
                  </v-icon>
                </v-list-tile-avatar>
               <span class='text--primary'>Ali Connors</span> 03451234567
                
              </v-list-tile>
            </v-list>
          
          </v-flex>
        </v-card>
       
       

      </v-flex>
     
</v-layout>


</v-container>
  
<Footer />
 
</div>
</template>
<script>
import Footer from './Footer.vue'
  export default {
    
   name: 'App',
  components: {
    Footer
  },

    data () {
      return {
       
        center: { lat: 45.508, lng: -73.587 },
      markers: [],
      places: [],
      currentPlace: null,

        email: '',
        rules: {
          required: value => !!value || 'Required.',
          counter: value => value.length <= 20 || 'Max 20 characters',
          email: value => {
            const pattern = /^(([^<>()[\]\\.,;:\s@"]+(\.[^<>()[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/
            return pattern.test(value) || 'Invalid e-mail.'
          }
        }
      };
    }}
  
  
  </script>