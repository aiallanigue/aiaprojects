<template>
  <v-app id="about">
    <NavBar />
    <v-container fluid>
      <div class="head">
        <v-row>
          <v-col cols="5">
            <div style="position: relative" class="mt-16">
              <h1 class="text-grey">Welcome to</h1>
              <h1 class="text-white">Car Customes</h1>
              <span class="text-grey">Your one-stop place for Lancer mods</span><br />

              <v-btn tile dark class="text-red mt-8" @click="scroll('contact')" variant="outlined">
                Contact me
              </v-btn>
            </div>
          </v-col>
          <v-col cols="2">
            <div
              style="
                position: absolute;
                z-index: 9999;
                bottom: 0;
                margin-left: auto;
                margin-right: auto;
                left: 0;
                right: 0;
                text-align: center;
              "
              class="mt-16"
            >
              <v-icon>fas fa-angle-double-down</v-icon>
            </div>
          </v-col>
          <v-col cols="5">
            <div style="position: relative; z-index: 9999" class="mt-16">
              <v-img src="por1.jpg" contain max-height="300"></v-img>
            </div>
          </v-col>
        </v-row>
      </div>
      <FooterView />
    </v-container>

    
  </v-app>


  

  
</template>

<script>
import { defineComponent } from "vue";
import NavBar from "../components/NavBar.vue";
import FooterView from "../components/FooterView.vue";

export default defineComponent({
  name: "AboutView",
  components: {
    NavBar,
    FooterView
  },
  methods: {
      scroll(refName) {
        const element = document.getElementById(refName);
        element.scrollIntoView({ behavior: "smooth" });
      },
    },
});
</script>
