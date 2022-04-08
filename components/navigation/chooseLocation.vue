<template>
  <v-card width="100%" class="white">
    <v-toolbar class="background" flat>
      <v-toolbar-title class="black--text">
        Choose your location
      </v-toolbar-title>
    </v-toolbar>
    <v-card-subtitle class="grey--text mt-4">
      Delivery options and delivery speeds may vary for different locations
    </v-card-subtitle>
    <v-row no-gutters class="d-flex justify-center">
      <v-btn 
        class="bright black--text" 
        rounded 
        @click="close"
        
      >
        Sign in to see your addresses
      </v-btn>
    </v-row>
    
    <v-divider class="my-4 background" />
    <v-card-subtitle class="grey--text d-flex justify-center">
      or enter a US zip code
    </v-card-subtitle>
    <v-row no-gutters class="mx-2 d-flex justify-center">
      <v-col cols="12" lg="7">
        <v-text-field light solo class="" />
      </v-col>
      <v-col cols="12" lg="3">
        <v-btn block class="background black--text mx-4 mt-1">Apply</v-btn>
      </v-col>
    </v-row>
    <v-divider class="my-4 background" />
    <v-card-subtitle class="grey--text d-flex justify-center">
      or
    </v-card-subtitle>
    <v-row class="mx-5" no-gutters>
      <v-select dense solo light placeholder="Ship outsite the US" />
    </v-row>
    <v-row class="d-flex justify-end pb-4 pr-4" no-gutters>
      <v-btn class="bright black--text" @click="close">Done</v-btn>
    </v-row>
  </v-card>
</template>
<script>
export default {
  methods: {
    close(){
      this.$emit('closeLocation')
    },
  }
}
</script>