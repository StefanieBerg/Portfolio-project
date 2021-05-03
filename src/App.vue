<template>
  <v-app>
    <v-app-bar
      app
      flat>
      
      <Header/>
    </v-app-bar>
    <v-container fluid>
      <router-view></router-view> 
    </v-container>  
     <v-footer>
      <Footer/>
    </v-footer>
  </v-app>
</template>

<script>
import Header from './components/Header';
//import Footer from './components/Footer';

export default {
  name: 'App',

  components: {
    Header,
    //Footer,
  },

  data: () => ({
    //
  }),
};
</script>


<style>
  #app{
  font-family: 'Raleway';
  color:#222;
  font-size: 20px !important;
  font-weight: 300;

   }

  .container{
   padding:0;
   max-width: 100% !important;
  }
</style>