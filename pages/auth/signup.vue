<template>
<v-container fluid class="white pb-0">
  


  <v-row no-gutters class="d-flex justify-center mt-5 pb-10">
    <v-col cols="12" lg='4' class="d-flex justify-center">
      <v-card class="white">
    <v-row>
      <v-card-title class="black--text display-1 ml-2">Create Account</v-card-title>
      
    </v-row>
    <v-row no-gutters class="my-0 py-0">
      <v-card-subtitle class="mb-0 pb-0 mt-3 font-weight-bold black--text">
        Your Name
      </v-card-subtitle>
    </v-row>
    <v-row no-gutters class="my-0 py-0">
      <v-text-field class="mx-4" solo light />
    </v-row>
    <!-- EMAIL --> 
    <v-row no-gutters class="my-0 py-0">
      <v-card-subtitle class="mb-0 pb-0 mt-3 font-weight-bold black--text">
        Mobile number or email
      </v-card-subtitle>
    </v-row>
    <v-row no-gutters class="my-0 py-0">
      <v-text-field class="mx-4"  solo light />
    </v-row>
    <!-- EMAIL --> 
    <v-row no-gutters class="my-0 py-0">
      <v-card-subtitle class="mb-0 pb-0 mt-3 font-weight-bold black--text">
        Password
      </v-card-subtitle>
    </v-row>
    <v-row no-gutters class="my-0 py-0">
      <v-text-field class="mx-4 py-0" placeholder="At least 6 characters" solo light />
    </v-row>
    <!-- Password confirm --> 
    <v-row no-gutters class="my-0 py-0">
      <v-card-subtitle class="mb-0 pb-0 mt-3 font-weight-bold black--text">
        Re-enter password
      </v-card-subtitle>
    </v-row>
    <v-row no-gutters class="my-0 py-0">
      <v-text-field class="mx-4" solo light />
    </v-row>
    <v-row no-gutters class="mx-4">
      <v-btn block class="bright black--text">Continue</v-btn>
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
    <v-divider inset class="background my-8" />
    <v-row no-gutters class="py-0">
      <v-card-subtitle class="black--text py-0">
        Already have an account?
        <v-btn text class="ablue--text pa-0" to="/auth/signin">Sign In</v-btn>
        <v-icon small color='ablue'>mdi-menu-right</v-icon>
      </v-card-subtitle>
    </v-row>
     <v-row no-gutters class="pt-0 pb-6">
      <v-card-subtitle class="black--text py-0">
        Buying for Work?
        <v-btn text class="ablue--text pa-0" to="/">Buying for Work?</v-btn>
        <v-icon small color='ablue'>mdi-menu-right</v-icon>
      </v-card-subtitle>
    </v-row>
  </v-card>
 
    </v-col>
  </v-row>
  
  <v-divider class='black--text mt-10' />
  <v-row class="background d-flex justify-center">
    <v-card-subtitle class="ablue--text">
      <nuxt-link 
        class="ablue--text text-decoration-none" 
        to="/policies/conditions-of-use"
      >
        Conditions of Use
      </nuxt-link>
    </v-card-subtitle>
    <v-card-subtitle class="ablue--text">
      <nuxt-link 
        class="ablue--text text-decoration-none" 
        to="/policies/privacy-notice"
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