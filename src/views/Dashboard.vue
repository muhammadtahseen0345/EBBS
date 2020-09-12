<template>

  <div class="Dashboard">
  
     
    <v-carousel >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    > 
   </v-carousel-item></v-carousel>
   <br />
   <br />

<v-container grid-list-md >
    <v-layout row wrap>

<v-flex xs12 sm6>
 <v-img src="https://cdn.vuetifyjs.com/images/parallax/material2.jpg"></v-img>
</v-flex>
<v-flex  class="blue lighten-2" xs12 sm6 text-xs-center>
  
<p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nisi numquam dolorem neque, dolor pariatur aperiam quis? Eaque nihil quia officiis in. Animi, minima. Quas distinctio doloremque sint laborum est dolorem.
  Lorem ipsum dolor sit amet consectetur adipisicing elit. Modi, doloribus in? Omnis provident, possimus esse impedit laborum aperiam, eligendi perspiciatis, commodi quod nisi reiciendis vitae harum magni explicabo architecto autem.
  Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates, eligendi! Sunt consequuntur molestiae blanditiis quidem, inventore reprehenderit cupiditate fugiat distinctio est. Aperiam ex rerum odio aliquid reiciendis animi, similique sapiente?

<v-btn outline @click="$router.push('about')">Hello</v-btn>
</p>
</v-flex>
</v-layout>
   </v-container>

<v-container grid-list-md >
  <v-layout row wrap>
      <v-flex xs12 sm2><v-spacer></v-spacer></v-flex>
<v-flex xs12 sm8 text-xs-center>
  
    <h1>Activities</h1>
  <p>EBBS(Education Builds the Bases of Society) is in the business of changing and shaping lives. The work we do at our
Organisation is aimed at providing a holistic approach to solving some of our society’s biggest challenges. We make sure our partners are
empowered by creating opportunities for individuals and communities.</p>


</v-flex>  
  </v-layout>    
</v-container>  
  
<v-container grid list-md>
    <v-layout row wrap>

<v-flex xs12 sm6>
  <v-img src="https://cdn.vuetifyjs.com/images/parallax/material2.jpg">
  <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nihil porro a placeat nobis asperiores odit fugit veniam iure eius earum necessitatibus aperiam aliquam, corrupti odio nisi ad veritatis. Molestiae, eveniet.</p>
</v-img>
</v-flex>
 
 
    
   <v-flex xs12 sm6>
  <v-img src="https://cdn.vuetifyjs.com/images/parallax/material2.jpg">
  <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nihil porro a placeat nobis asperiores odit fugit veniam iure eius earum necessitatibus aperiam aliquam, corrupti odio nisi ad veritatis. Molestiae, eveniet.</p>
</v-img>
</v-flex>
 
    
    </v-layout>
</v-container>
<br/>

<v-divider
            class="mx-auto"
            style="width: 800px; "
          />
<br/>
 <v-container >
    <v-layout>
      <v-flex xs6 >
        <v-img
          src="https://cdn.vuetifyjs.com/images/parallax/material2.jpg"
          gradient="to top right, rgba(100,115,201,.33), rgba(25,32,72,.7)"
        ></v-img>
      </v-flex>
         Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eaque itaque rem ab repellendus! Mollitia repellendus praesentium libero natus accusamus, tenetur, expedita magnam deleniti sapiente, optio iure molestiae debitis. Nobis, aspernatur!
      

     
    </v-layout>
  </v-container>

<v-divider
            class="mx-auto"
            style="width: 800px; "
          />
<br/>
 <v-container >
    <v-layout>
      <v-flex xs6 >
        <v-img
          src="https://cdn.vuetifyjs.com/images/parallax/material2.jpg"
          gradient="to top right, rgba(100,115,201,.33), rgba(25,32,72,.7)"
        ></v-img>
      </v-flex>
         Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eaque itaque rem ab repellendus! Mollitia repellendus praesentium libero natus accusamus, tenetur, expedita magnam deleniti sapiente, optio iure molestiae debitis. Nobis, aspernatur!
      

     
    </v-layout>
  </v-container>

  <v-divider
            class="mx-auto"
            style="width: 800px; "
          />
<br/>
 <v-container >
    <v-layout text-xs-center>
      <v-flex xs6 >
        <v-img
          src="https://cdn.vuetifyjs.com/images/parallax/material2.jpg"
          gradient="to top right, rgba(100,115,201,.33), rgba(25,32,72,.7)"
        ></v-img>
      </v-flex>
         Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eaque itaque rem ab repellendus! Mollitia repellendus praesentium libero natus accusamus, tenetur, expedita magnam deleniti sapiente, optio iure molestiae debitis. Nobis, aspernatur!
      

     
    </v-layout>
  </v-container>

  <v-divider
            class="mx-auto"
            style="width: 800px; "
          />
<br/>
 <v-container >
    <v-layout>
      <v-flex xs6 >
        <v-img
          src="https://cdn.vuetifyjs.com/images/parallax/material2.jpg"
          gradient="to top right, rgba(100,115,201,.33), rgba(25,32,72,.7)"
        ></v-img>
      </v-flex>
         Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eaque itaque rem ab repellendus! Mollitia repellendus praesentium libero natus accusamus, tenetur, expedita magnam deleniti sapiente, optio iure molestiae debitis. Nobis, aspernatur!
      

     
    </v-layout>
  </v-container>


<Footer />

  </div>
  
</template>
<script>
  import Footer from './Footer.vue'
  

 export default {
  videoId: 'https://youtu.be/foT-z4bymb0',
     name: 'App',
  components: {
    Footer,
    
  },

     
    data: () => ({
     
      drawer:false,
      email:'',
      links:[
          {icon:'person', text:'Shortcuts'
         }
        ],
      
      admins: [
        /*['Team', 'people_outline'],*/
        {icon:'people_outline', text:'Team', route:'/team'
         },
         {icon:'people_outline', text:'Trainer', route:'/trainer'
         }
        /*['Trainers', 'settings']*/
      ],

     

      cruds: [
        /*['Work With Us', 'add'],
        ['Collabrations/Partners', 'insert_drive_file'],
        ['Alumni/Success Stories', 'update'],*/
        {icon:'add', text:'Work With Us', route:'/Work'
         },
         {icon:'people_outline', text:'Trainer', route:'/trainer'
         }
      ],
      
      items: [
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg'
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg'
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg'
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg'
          }
        ],
        methods: {
      next () {
        alert('You clicked next!')
      },
      method (url) {
      this.videoId = this.$youtube.getIdFromURL(url)
      this.startTime = this.$youtube.getTimeFromURL(url)
    }
    }
      
       
    })
  }
</script>
<style lang="stylus">

  #footer
    a
      opacity: .8
      text-decoration: none
      &:hover
        color: #FFF
        opacity: 1
    .v-text-field--rounded
      margin-bottom: 16px
      .v-input__slot
        border-radius: 28px
      .v-text-field__slot,
      .v-label
        padding-left: 8px
      .v-btn
        margin: 0
        border-top-right-radius: 28px
        border-bottom-right-radius: 28px
        box-shadow: none
        height: 48px
        margin-right: -12px
        padding-top: 2px
</style>