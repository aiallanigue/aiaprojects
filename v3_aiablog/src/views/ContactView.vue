<template>
    <v-app id="contact">
      <NavBar />
      <v-container fluid>
        
        <GoogleMap
    api-key="AIzaSyD3xSh-SxWxKzYu0NqcNyFgTtZynAKm8Wc"
    style="width: 100%; height: 500px"
    :center="center"
    :zoom="15"
    >
      <Marker :options="{ position: center }" />
    </GoogleMap>

        <v-col cols="12" sm="12" class="px-16" id="contact">
            <v-row>
              <v-col cols="12" sm="4">
                <div class="child">
                  <h1>Contact info.</h1>
                  <v-btn
                    icon="fas fa-map-marker-alt"
                    color=""
                    class="mt-10"
                    variant="outlined"
                    href="https://www.google.com/maps/@14.027996,121.1627373,20.25z"
                    target="_blank"
                  ></v-btn
                  ><br />
                  <span class="text-caption">Manila, Philippines</span
                  ><br />
                  <v-btn
                    icon="fas fa-phone-alt"
                    color=""
                    class="mt-10"
                    variant="outlined"
                  ></v-btn
                  ><br />
                  <span class="text-caption">+639178276302</span> <br />
                  <v-btn
                    icon="fas fa-envelope"
                    color=""
                    class="mt-10"
                    variant="outlined"
                    href="allanallanigue@gmail.com"
    
                  ></v-btn
                  ><br />
                  <span class="text-caption">allanallanigue@gmail.com</span> <br />
                </div>
              </v-col>
              <v-col cols="12" sm="8">
                <h1 class="mt-8">Send your message</h1>
                <v-divider></v-divider>
                <span class="text-caption"
                  >Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt
                  fugiat officia, odio eaque exercitationem libero nesciunt placeat,
                  repellat obcaecati sed tenetur! Est labore aliquam amet
                  consequatur necessitatibus fugit obcaecati facilis!</span
                >
                <v-row class="mt-10">
                  <v-col cols="12" sm="6">
                    <v-text-field
                      label="Name"
                      persistent-hint
                      variant="outlined"
                    ></v-text-field>
                  </v-col>
                  <v-col cols="12" sm="6">
                    <v-text-field
                      label="Phone No"
                      persistent-hint
                      variant="outlined"
                    ></v-text-field>
                  </v-col>
                </v-row>
                <v-textarea
                  label="Message"
                  persistent-hint
                  variant="outlined"
                ></v-textarea>
                <v-btn color="#ff3535" class="mt-2">Submit Now</v-btn>
              </v-col>
            </v-row>
          </v-col>
        <FooterView />
      </v-container>
    </v-app>
  
  </template>
  
  <script>
  
  import { defineComponent } from "vue";
  import NavBar from "../components/NavBar.vue";
  import FooterView from "../components/FooterView.vue";
  import { GoogleMap, Marker } from 'vue3-google-map'
  
  export default defineComponent({
    name: "ContactView",
    
    components: {
      NavBar,
      FooterView,
      GoogleMap, 
      Marker,
    },
    setup() {
    const center = { lat: 14.027895872291703, lng: 121.16270912828324 }

    return { center }
  },
    
  });
  </script>
  