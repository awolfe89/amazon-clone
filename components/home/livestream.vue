<template>
  <v-card width="100%" flat class="mb-10 mt-4 white">
    <v-row no-gutters>
      <v-card-title class="display-1 black--text">Amazon Live | Shop Livestreams 
        <span class=" ml-2 mt-2 subtitle-2 secondary--text">See More from Amazon Live</span>
      </v-card-title>
    </v-row>
    <v-row class="mx-2 d-flex justify-space-between">
      <v-col cols="12" lg='3'>
        <v-card width="100%" height="400" class="white mx-2" flat>
          <v-card>
          <v-img
            src="https://picsum.photos/510/300?random"
            aspect-ratio="1.7"
            class="mx-2"
          />
          <v-overlay
     
            absolute
            color="#036358"
          >
            <v-btn>
              <v-icon>mdi-arrow-expand-all</v-icon>
              Watch Now</v-btn>
          </v-overlay>
          </v-card>
          
        <v-card-subtitle class="primary--text">Shop More</v-card-subtitle>
        </v-card>
      </v-col>

      <v-col cols="12" lg='9' md="2" sm="6">
         <v-slide-group
          v-model="model"

        >
          <v-slide-item
            v-for="n in 15"
            :key="n"
          >
            <v-card
              class="ma-4"
              height="200"
              width="100"
            >
              <v-row
                class="fill-height"
                align="center"
                justify="center"
              >
              </v-row>
            </v-card>
          </v-slide-item>
        </v-slide-group>
      </v-col>
    </v-row>
  </v-card>
</template>