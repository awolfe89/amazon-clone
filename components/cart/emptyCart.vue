<template>
  <v-card width="100%" class="white" flat>
    <v-row>
      <v-col cols="12" lg='4'>
        <v-img
          src="https://picsum.photos/510/300?random"
          aspect-ratio="1.7"
          class="ml-2"
        />
      </v-col>
      <v-col cols="12" lg='8'>
        <v-card class="white" flat>
          <v-card-title class="black--text">
            You Amazon Cart is empty
          </v-card-title>
          <v-card-subtitle class="ablue--text">
            Shop today's deals
          </v-card-subtitle>
          <v-row class="mt-1 mx-4">
            <v-btn 
              class="bright black--text mx-2"
              @click="$router.push('/auth/signin')"
            >
              sign in to your account
            </v-btn>
            <v-btn 
              class="background black--text"
              @click="$router.push('/auth/signup')"
            >
              sign up now
            </v-btn>
          </v-row>
        </v-card>
      </v-col>
    </v-row>
  </v-card>
</template>