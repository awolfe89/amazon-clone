<template>
<v-container fluid class="background">
  <v-row class="white d-flex justify-center ma-0 pb-5">
    <v-col cols="12" lg='6'>
      <v-card elevation="3" class="white">
        <v-row no-gutters>
        <v-card-title class="black--text display-3">Sign In</v-card-title>
        <v-card-subtitle class="black--text font-weight-bold ma-0">
          Email or mobile phone number
          <v-text-field outlined solo light/>
        </v-card-subtitle>
        <v-btn class="bright black--text mx-4" block>Sign In</v-btn>
        </v-row>
        
      </v-card>
    </v-col>
  </v-row>
  <v-divider class='black--text' />
  <v-row class="background d-flex justify-center">
    <v-card-subtitle class="ablue--text">Conditions of Use</v-card-subtitle>
    <v-card-subtitle class="ablue--text">Privacy Notice</v-card-subtitle>
    <v-card-subtitle class="ablue--text">Help</v-card-subtitle>
  </v-row>
  <v-row class="background d-flex justify-center my-0 py-0">
    <v-card-subtitle class="black--text">© 1996-2022, Amazon.com, Inc. or its affiliates</v-card-subtitle>
  </v-row>
</v-container>
  
</template>