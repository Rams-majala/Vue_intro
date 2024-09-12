<template>
   <v-app-bar
      app
      color="primary"
      dark
    >
    <v-row class="d-flex align-center mx-10">   
    <router-link class="white--text mx-3 text-decoration-none" to="/"><h1>Gerage</h1></router-link>
   <v-spacer></v-spacer> 
     <router-link v-for="(detail, id) in details" :key="id"  class="white--text mx-4 text-decoration-none" :to="detail.destination">{{ detail.name }}</router-link>

 </v-row>


    
    </v-app-bar>
</template>
  
<script>
  // import MainButton from "./MainButton.vue";
  export default {
    name: "HeaderComponent",
    components: {
      // MainButton,
    },
    data() {
      return {
        details:[
          {
            name: 'Home',
            destination: '/',

          },
          {
            name: 'About Us',
            destination: '/about'
          },
          {
            name: 'Contact Us',
            destination: '/contact'
          }
        ],
        path: '/about'
        
  
        
      };
    },
    methods: {
      goToBookForm() {
        this.$router.push("/Booknow");
      },
    },
  };
  </script>
  