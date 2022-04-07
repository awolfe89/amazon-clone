<template>
  <v-card flat class="white mt-7">
    <v-card-text class="black--text font-weight-bold">
      Customers Who Bought Items in Your Recent History Also Bought
    </v-card-text>
    <!-- ITEM ONE --> 
    <v-row class="">
      <v-col cols='5'>
        <v-img
          src="https://picsum.photos/510/300?random"
          aspect-ratio="1.7"
          class="ml-2"
          height="100"
          width="200"
        />  
      </v-col>
      <v-col cols="6">
        <v-card-text class="ablue--text ma-0 pa-0">SELETERM 1/0 AWG...</v-card-text>
        <v-row class="mt-0">
          <v-rating
            v-model="rating"
            background-color="warning"
            dense
            half-increments
            color="warning"
            size="20"
            class="py-0 my-0 ml-3"
          />
          <span class="ablue--text text-caption ml-2 mt-1">
            9,164
          </span>
        </v-row>
        <v-card-text class="error--text font-weight-bold mt-3 pa-0">
          $10.59
        </v-card-text>
        <v-btn class="bright black--text mt-1" small>
          Add to Cart
        </v-btn>
      </v-col>
    </v-row>
    <!-- ITEM ONE --> 
    <v-row class="">
      <v-col cols='5'>
        <v-img
          src="https://picsum.photos/510/300?random"
          aspect-ratio="1.7"
          class="ml-2"
          height="100"
          width="200"
        />  
      </v-col>
      <v-col cols="6">
        <v-card-text class="ablue--text ma-0 pa-0">SELETERM 1/0 AWG...</v-card-text>
        <v-row class="mt-0">
          <v-rating
            v-model="rating"
            background-color="warning"
            dense
            half-increments
            color="warning"
            size="20"
            class="py-0 my-0 ml-3"
          />
          <span class="ablue--text text-caption ml-2 mt-1">
            9,164
          </span>
        </v-row>
        <v-card-text class="error--text font-weight-bold mt-3 pa-0">
          $10.59
        </v-card-text>
        <v-btn class="bright black--text mt-1" small>
          Add to Cart
        </v-btn>
      </v-col>
    </v-row>
    <!-- ITEM ONE --> 
    <v-row class="">
      <v-col cols='5'>
        <v-img
          src="https://picsum.photos/510/300?random"
          aspect-ratio="1.7"
          class="ml-2"
          height="100"
          width="200"
        />  
      </v-col>
      <v-col cols="6">
        <v-card-text class="ablue--text ma-0 pa-0">SELETERM 1/0 AWG...</v-card-text>
        <v-row class="mt-0">
          <v-rating
            v-model="rating"
            background-color="warning"
            dense
            half-increments
            color="warning"
            size="20"
            class="py-0 my-0 ml-3"
          />
          <span class="ablue--text text-caption ml-2 mt-1">
            9,164
          </span>
        </v-row>
        <v-card-text class="error--text font-weight-bold mt-3 pa-0">
          $10.59
        </v-card-text>
        <v-btn class="bright black--text mt-1" small>
          Add to Cart
        </v-btn>
      </v-col>
    </v-row>
    <!-- ITEM ONE --> 
    <v-row class="">
      <v-col cols='5'>
        <v-img
          src="https://picsum.photos/510/300?random"
          aspect-ratio="1.7"
          class="ml-2"
          height="100"
          width="200"
        />  
      </v-col>
      <v-col cols="6">
        <v-card-text class="ablue--text ma-0 pa-0">SELETERM 1/0 AWG...</v-card-text>
        <v-row class="mt-0">
          <v-rating
            v-model="rating"
            background-color="warning"
            dense
            half-increments
            color="warning"
            size="20"
            class="py-0 my-0 ml-3"
          />
          <span class="ablue--text text-caption ml-2 mt-1">
            9,164
          </span>
        </v-row>
        <v-card-text class="error--text font-weight-bold mt-3 pa-0">
          $10.59
        </v-card-text>
        <v-btn class="bright black--text mt-1" small>
          Add to Cart
        </v-btn>
      </v-col>
    </v-row>
  </v-card>
</template>

<script>
export default {
  data(){
    return {
      rating: 4.5
    }
  }
}
</script>