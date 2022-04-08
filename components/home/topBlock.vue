<template>
  <v-row no-gutters class="pt-5">
    <v-col cols='8' class="mx-0">
      <v-row class=" mx-2 d-flex justify-center">
        <v-col cols="4" >
          <v-card class="white" width="400" height="500">
            <v-card-title class="black--text font-weight-bold">Premium Dress</v-card-title>
            <v-img
              lazy-src="https://picsum.photos/id/11/10/6"
              max-height="150"
              max-width="250"
              src="https://picsum.photos/id/11/500/300"
            ></v-img>
            <v-card-subtitle class="primary--text">Shop More Styles</v-card-subtitle>
          </v-card>
        </v-col>
         <v-col cols="4" >
          <v-card class="white" height="500">
            <v-card-title class="black--text font-weight-bold">Premium Dress</v-card-title>
            <v-img
              lazy-src="https://picsum.photos/id/11/10/6"
              max-height="150"
              max-width="250"
              src="https://picsum.photos/id/11/500/300"
            ></v-img>
            <v-card-subtitle class="primary--text">Shop More Styles</v-card-subtitle>
          </v-card>
        </v-col>
         <v-col cols="4" >
          <v-card class="white" height="500">
            <v-card-title class="black--text font-weight-bold">Premium Dress</v-card-title>
            <v-img
              lazy-src="https://picsum.photos/id/11/10/6"
              max-height="150"
              max-width="250"
              src="https://picsum.photos/id/11/500/300"
            ></v-img>
            <v-card-subtitle class="primary--text">Shop More Styles</v-card-subtitle>
          </v-card>
        </v-col>
         
      </v-row>
    </v-col>
    <!--- RIGHT HAND AREA --> 
    <v-col cols="4" class="mx-0">
      <v-card width="100%" class="white">
        <v-card-text class="pt-4 black--text font-weight-bold">
          Sign in for the best experience
        </v-card-text>
        <v-row no-gutters class="pb-10 d-flex justify-center">
            <v-btn class=" black--text" large color="bright" to="/auth/signup">Sign in securely</v-btn>
        </v-row>
        
      </v-card>
      <!-- <v-card>
        <v-card-text>byebye</v-card-text>
      </v-card> -->
    </v-col>
  </v-row>
</template>