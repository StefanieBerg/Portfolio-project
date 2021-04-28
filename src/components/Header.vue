<template>
  <v-container>
   <v-toolbar flat>
      <v-toolbar-title>Portfolio</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-toolbar-items class="hidden-xs-only">
        <v-btn text>
          <router-link to="/">Home</router-link>
        </v-btn>

        <v-btn text>
          <router-link to="/myprojects">My projects</router-link>
        </v-btn>

        <v-btn text>
          <router-link to="/contact">Contact</router-link>
        </v-btn>
      </v-toolbar-items>
      <div class="hidden-sm-and-up">
        <v-menu offset-y>
          <template v-slot:activator="{ on }">
            

              <v-app-bar-nav-icon v-on="on"></v-app-bar-nav-icon>
           
          </template>
      <v-list class="responsiveMenu">
        <v-list-item>
          <v-list-item-title><router-link to="/">Home</router-link></v-list-item-title>
        </v-list-item>
        <v-list-item>
          <v-list-item-title><router-link to="/myprojects">My projects</router-link></v-list-item-title>
        </v-list-item>
        <v-list-item>
          <v-list-item-title><router-link to="/contact">Contact</router-link></v-list-item-title>
        </v-list-item>
        
      </v-list>
    </v-menu>
      </div>
    </v-toolbar>
  </v-container>
</template>

<script>
  export default {
    name: 'Header',

    data: () => ({
      
    }),
  }
</script>

<style lang="scss">
  header {
    .v-toolbar__title {
      font-weight: 600;
      text-transform: uppercase;
    }
  
    .v-toolbar__content {
      @media only screen and (max-width: 599px) {
        padding: 0;
      }
    }
  }
  .v-toolbar.items {

    .v-btn {
      color: black;
    }
  }
</style>
