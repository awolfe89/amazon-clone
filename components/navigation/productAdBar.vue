<template>
<v-container fluid class="pa-0 ma-0">
  <v-row dense class="background">
    <v-col cols='12' lg='3'></v-col>
    <v-col cols='12' lg='6'>
      <v-card-text class="black--text">Cobra PRO 1500W Professional Grade Power...</v-card-text>
    </v-col>
    <v-col cols='12' lg='3'>
      <v-row>
       <v-rating
          v-model="rating"
          background-color="warning"
          color="warning"
          size="20"
          class="pt-2 pb-0"
       />
       <v-card-subtitle class="subtitle-2 grey--text pb-0">353</v-card-subtitle>
      </v-row>
      <v-row>
        <v-card-subtitle class="pt-0 subtitle-2 error--text">$199.99</v-card-subtitle>
      </v-row>
    </v-col>
  </v-row>
  </v-container>
</template>
<script>
export default {
  data() {
    return { 
      rating: 4,
    }
  }
}
</script>