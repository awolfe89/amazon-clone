<template>
<v-container fluid class="white pb-0">
  


  <v-row no-gutters class="d-flex justify-center mt-5 pb-10">
    <v-col cols="12" lg='4'>
      <v-card class="white">
    <v-row>
      <v-card-title class="black--text display-1 ml-2">Sign In</v-card-title>
      
    </v-row>
    <v-row no-gutters>
      <v-card-subtitle class="mb-0 pb-0 mt-3 font-weight-bold black--text">
        Email or mobile phone number
      </v-card-subtitle>
      
    </v-row>
    <v-row no-gutters class="my-0 py-0">
      <v-text-field class="mx-4" label="email" solo light />
      
    </v-row>
    <v-row no-gutters class="mx-4">
      <v-btn block class="bright black--text">Sign In</v-btn>
    </v-row>
    <v-row no-gutters>
      <v-card-subtitle class="black--text">
      By Continuing, you agree to Amazon's 
      <nuxt-link 
        class="ablue--text text-decoration-none" 
        to="/policies/conditions-of-use"
      >
        Conditions of Use
      </nuxt-link>
      and
      <nuxt-link 
        class="ablue--text text-decoration-none" 
        to="/policies/privacy-notice"
      >
        Privacy Notice
      </nuxt-link>
      </v-card-subtitle>
    </v-row>
    <v-row no-gutters>
      <v-card-subtitle class="ablue--text">
        <v-icon small color='ablue'>mdi-menu-right</v-icon>
         Need Help?</v-card-subtitle>
    </v-row>
  </v-card>
  <v-row no-gutters class='d-flex justify-center mt-6 pb-0'>
    <v-card-subtitle class="black--text">New to Amazon?</v-card-subtitle>
  </v-row>
   <v-row no-gutters class='d-flex justify-center'>
    <v-btn block class="background black--text mx-6" to='/auth/signup'>Create Your Amazon Account</v-btn>
  </v-row>
    </v-col>
  </v-row>
  
  <v-divider class='black--text mt-10' />
  <v-row class="background d-flex justify-center">
    <v-card-subtitle class="ablue--text">
      <nuxt-link class="ablue--text text-decoration-none" to="/policies/conditions-of-use">
        Conditions of Use
      </nuxt-link>
    </v-card-subtitle>
    <v-card-subtitle class="ablue--text">
      <nuxt-link 
        class="ablue--text text-decoration-none" 
        to="/policies/conditions-of-use"
      >
        Privacy Notice
      </nuxt-link>
    </v-card-subtitle>
    <v-card-subtitle class="ablue--text">Help</v-card-subtitle>
  </v-row>
  <v-row class="background d-flex justify-center my-0 pt-0 pb-10">
    <v-card-subtitle class="black--text">© 1996-2022, Amazon.com, Inc. or its affiliates</v-card-subtitle>
  </v-row>
</v-container>
  
</template>