<template>
  <v-card class="white" light> 
          <v-card-title class="black--text">$00.00</v-card-title>
          <v-card-subtitle class="black--text pb-0">& <span class="ablue--text">FREE Returns</span> </v-card-subtitle>
          <v-card-subtitle class="ablue--text pt-0">
            FREE delivery <span class="black--text font-weight-bold">Tuesday, March 10</span>
          </v-card-subtitle>
          <v-card-subtitle class="black--text pt-0">
            Or fastest delivery <span class="black--text font-weight-bold">
              Saturday March 9.
            </span>
            Order within <span class="green--text">10hrs 1 min</span>
          </v-card-subtitle>
          <v-card-subtitle class="ablue--text subtitle-2 pt-0">
            <v-icon small color="secondary">mdi-google-maps</v-icon>
            select delivery location
          </v-card-subtitle>
          <v-card-text class="green--text font-weight-bold">In Stock.</v-card-text>
          <v-select placeholder="Qty 1" class="mx-3" solo />
          <v-card flat class="mx-2">
            <v-btn block rounded class="black--text accent my-3 px-2">Add to Cart</v-btn>
            <v-btn block rounded class="black--text warning my-3 px-2">Buy Now</v-btn>
          </v-card>
          
          <v-icon color="grey" class="ml-2">mdi-lock</v-icon>
          <span class="ablue--text">Secure Transaction</span>

          <v-card-subtitle class="grey--text subtitle-2 pb-0">Ships From <span class="black--text">Amazon</span> </v-card-subtitle>
          <v-card-subtitle class="grey--text subtitle-2 pt-0">Sold by <span class="ablue--text">zdcsdvsdv</span> </v-card-subtitle>

          <v-card-text class="black--text">Return Policy:
            <span class="ablue--text">Eligible for Return, Refund or Replacement within 30 days of receipt</span>
          </v-card-text>
          <v-card>
            <v-card-text class="ablue--text">Prime</v-card-text>
          <v-card-text class="black--text font-weight-bold pb-0 pt-0">Enjoy fast, FREE delivery, exclusive deals and award-winning movies & TV shows with prime</v-card-text>
          <v-card-subtitle class="black--text pt-0">
            <span class="ablue--text">Try Prime</span>
            and start saving today with 
            <span class="font-weight-bold">Fast, FREE Delivery</span>
          </v-card-subtitle>
          </v-card>
          
          <v-checkbox class="mx-2" label="Add a gift reciept for easy returns" />
          <v-btn elevation="2" color='background' block class=" black--text">Add to List</v-btn>
      </v-card>
        
</template>