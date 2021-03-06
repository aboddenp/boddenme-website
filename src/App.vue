<template>
  <v-app>
    <SideBar></SideBar>
    <v-main>
      <v-parallax  src="./assets/computer.jpg">
        <v-row class="mt-6" >
          <v-col class="text-center" >
            <v-avatar size="150"
              color="grey"
            >
              <v-img src="./assets/me.jpg"></v-img>
            </v-avatar>

            <v-sheet
                class=" mt-5 mx-auto py-5"
                color="white"
                elevation="3"
                width="250"
                rounded="lg"
                height="auto"
              >
              <div class=" pt-3 text--primary text-h4">Aster Bodden</div>
              <div class="overline text--secondary ">Software Developer</div>
              <div class="caption text--secondary pa-5">"A machine that turns coffee into code"</div>
            </v-sheet>
            
          </v-col>
        </v-row>

      </v-parallax>

    </v-main>
  </v-app>
</template>

<script>
import SideBar from './components/SideBar.vue';

export default {
  name: 'App',

  components: {
    SideBar
  },

  data: () => ({}),
};
</script>
