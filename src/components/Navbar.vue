<template>
  <nav>
    <v-toolbar app height="90px">
      <v-toolbar-side-icon class="grey--text" @click="drawer =!drawer"></v-toolbar-side-icon>
      <v-toolbar-title class="text-uppercase grey--text">
       <span class="font-weight-light"><v-img  width="170px" height="" :src="image_src"></v-img></span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn flat @click="$router.push('about')">About</v-btn>
      <v-btn flat @click="$router.push('about')">Network</v-btn>
      <v-btn flat @click="$router.push('contact')">Contact</v-btn>
    </v-toolbar>

    <v-navigation-drawer app v-model="drawer" class='blue'>
      
      
      <v-list>
        <v-list-tile v-for="link in links" :key="link.text" route :to="link.route">
          <v-list-tile-action>
            <v-icon class="white--text">{{link.icon}}</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title class="white--text">{{link.text}}</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
     
     
      
    </v-navigation-drawer>
  </nav>
</template>


<script>
export default {
  data() {
    return {
      drawer: false,
       image_src: require("../assets/EBBS logo.png"),
      links: [
        { icon: "dashboard", text: "Dashboard", route: "/" },
        { icon: "folder", text: "My Projects", route: "/projects" },
        { icon: "person", text: "Team", route: "/team" },
        { icon: "note_add", text: "Trainer", route: "/Trainer" },
        { icon: "search", text: "Alumni/Success Stories", route: "/dummy" },
         { icon: "search", text: "Collabration/Partners", route: "/dummy" },
        { icon: "search", text: "Work With Us", route: "/dummy" },
       
      ]
    };
  }
};
</script>
