<template>
    <v-app-bar app color="black" dark flat class="px-12" >
      <v-btn >
        <v-icon color="red" left class="mr-2">fas fa-signature</v-icon> CAR CUSTOMS
      </v-btn>
      
  
      <v-spacer></v-spacer>
      <router-link class="rtr-nav v-btn v-theme--light v-btn--density-default v-btn--size-default v-btn--variant-text" to="/">Home</router-link>
      <router-link class="rtr-nav v-btn v-theme--light v-btn--density-default v-btn--size-default v-btn--variant-text" to="/about">About</router-link>
      <!-- <v-btn text @click="scroll('home')" class="text-red">Home</v-btn>
      <v-btn text @click="scroll('about')"  >About</v-btn> -->
      <v-btn text class="rtr-nav v-btn v-theme--light v-btn--density-default v-btn--size-default v-btn--variant-text" @click="scroll('portfolio')"  >Parts</v-btn>
      <v-btn text class="rtr-nav v-btn v-theme--light v-btn--density-default v-btn--size-default v-btn--variant-text" @click="scroll('services')" > Services</v-btn>
      <v-btn text class="rtr-nav v-btn v-theme--light v-btn--density-default v-btn--size-default v-btn--variant-text" @click="scroll('page')"  > Testimonials</v-btn>
      <v-btn text class="rtr-nav v-btn v-theme--light v-btn--density-default v-btn--size-default v-btn--variant-text" @click="scroll('biog')"  > Gallery</v-btn>
      <router-link class="rtr-nav v-btn v-theme--light v-btn--density-default v-btn--size-default v-btn--variant-text" to="/contact">Contact</router-link>
      <!-- <v-btn text @click="scroll('contact')"  > Contact</v-btn> -->
    </v-app-bar>
  </template>
  
  <script>
  export default {
    methods: {
      scroll(refName) {
        const element = document.getElementById(refName);
        element.scrollIntoView({ behavior: "smooth" });
      },
    },
  };
  </script>
  
  <style scoped>
    .rtr-nav:hover {
      color: red;
    }
  </style>