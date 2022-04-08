<template>
<v-card width="100%" class="background" flat>
<v-row class="d-flex justify-center py-0">
    <v-card-subtitle class="black--text">See Personalized Recommendations</v-card-subtitle>
</v-row>
<v-row class="d-flex justify-center my-0">
    <v-btn color="accent" class="black--text" to="/auth/signin">Sign In</v-btn>
</v-row>
<v-row class="d-flex justify-center my-0">
    <v-card-subtitle class="black--text">New Customer?
      <nuxt-link 
        class="ablue--text text-decoration-none" 
        to="/auth/signup"
      >
        Start Here
      </nuxt-link>
    </v-card-subtitle>
  </v-row>
</v-card>
  
</template>