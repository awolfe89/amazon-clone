<template>
  <v-container fluid class="dark">
    <v-row class="dark" dense no-gutters>
      <v-app-bar flat class="dark py-2 my-2">
          <v-col cols="12" lg='1' md='2' sm="4" class="px-0">
              <v-card-title>AMAZON</v-card-title>
          </v-col>
          <v-col cols="12" lg='1' md='2' sm="4" class="px-0">
            <v-card-text class="font-weight-bold">
              <v-icon>mdi-google-maps</v-icon>
              Select Your Address
            </v-card-text>
          </v-col>
          <v-col cols="12" lg="6" md="4" sm="2">
            <v-text-field 
              outlined 
              placeholder="search" 
              prepend-inner-icon="mdi-magnify"
              class="mt-2"
              />
          </v-col>
          
          <v-col cols="1" class="px-0">
            <v-card-text class="my-0 py-0">Hello, sign in</v-card-text>
            <v-card-text class="my-0 py-0 font-weight-bold">Account & Lists</v-card-text>
          </v-col>
          <v-col cols="1" class="px-0">
            <v-card-text class="my-0 py-0">Returns</v-card-text>
            <v-card-text class="my-0 py-0 font-weight-bold">& Orders</v-card-text>
          </v-col>
          <v-col cols="1" class="px-0">
            <v-button icon>
              <v-icon color="warning" large>mdi-cart-outline</v-icon>
           <span>Cart</span>
            </v-button>
          </v-col>
      </v-app-bar>
    </v-row>
    <v-row>
      <v-toolbar dense flat class="primary">
        <v-app-bar-nav-icon @click="drawer = true" class="pr-0" />
        <v-card-subtitle class=" ml-0 pl-0 font-weight-bold">All</v-card-subtitle>
        <v-card-subtitle
          v-for="item in menu" :key="item"
        >
          {{item.name}}
        </v-card-subtitle>
      </v-toolbar>
    </v-row>
    <!-- MAIN MENU --> 
    <v-navigation-drawer
      v-model="drawer"
      app
      temporary
      clipped-left="clipped"
    >
      <MainMenu />
    </v-navigation-drawer>
  </v-container>
</template>

<script>
import MainMenu from '../navigation/mainMenu'
export default {
  components: {
    MainMenu
  },
  data() {
    return {
      drawer: false,
      menu: [
        {
          name: "Best Sellers"
        },
        {
          name: 'Amazon Basics'
        },
        {
          name: "New Releases"
        },
        {
          name: "Customer Service"
        },
        {
          name: "Today's Deals"
        },
        {
          name: "Prime"
        },
        {
          name: "Amazon Home"
        },
        {
          name: "Books"
        },
        {
          name: "Music"
        },
        {
          name: "Registry"
        },
        {
          name: "Fashion"
        },
        {
          name: "Kindle Books"
        },
        {
          name: "Gift Cards"
        },
        {
          name: "Toys & Games"
        },
        {
          name: "Sell"
        },
        {
          name: "Automotive"
        },
      ],

    }
  }
}
</script>