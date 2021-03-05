<template>
  <v-app>
    <v-app-bar
      app
      color="secondary"
      dark
    >
      <div class="d-flex align-center">
      
      <v-menu offset-y >
          <template v-slot:activator="{ on, attrs }">
            <v-btn
              dark
              v-bind="attrs"
              v-on="on"
              icon
            >
              <v-icon> mdi-menu </v-icon>
            </v-btn>
          </template>
           <v-list nav rounded>
            <v-list-item-group  >
                <v-list-item class="d-flex justify-center blue lighten-5" >
                  <v-icon >mdi-home</v-icon>
                </v-list-item>
                <v-list-item  class="px-6" v-for="info in nav_info" :key="info.name">
                  <v-list-item-icon><v-icon > {{info.icon}} </v-icon></v-list-item-icon>
                  <v-list-item-content>{{info.name}}</v-list-item-content>
                </v-list-item>
            </v-list-item-group>
           </v-list>
          </v-menu>
      </div>

      <v-spacer></v-spacer>

        <v-btn 
          icon
          href="https://www.linkedin.com/in/aster-bodden-pineda-35b386115/"
          target="_blank"
        >
          <v-icon> mdi-linkedin</v-icon>
        </v-btn>

        <v-btn 
          icon
          href="https://github.com/aboddenp/boddenme-website"
          target="_blank"
        >
          <v-icon> mdi-github</v-icon>
        </v-btn>
    </v-app-bar>

    <v-main>
    </v-main>
  </v-app>
</template>

<script>
// import SideBar from './components/SideBar';

export default {
  name: 'App',

  components: {
  },

  data: () => ({
    nav_info:[
      {
        icon:"mdi-forum",
        name:"About me"

      },
      {
        icon:"mdi-school",
        name:"Education"
      },
      {        
        icon:"mdi-wrench",
        name:"Skills"
      },
      {        
        icon:"mdi-bug",
        name:"Experience"
      },
      {        
        icon:"mdi-brightness-4",
        name:"Dark Mode"
      }
    ]
  }),
};
</script>
