<template>
  <v-container fluid class="dark">
    <v-row class="dark" dense no-gutters>
      <v-app-bar flat class="dark py-2 my-2">
          <v-col cols="12" lg='1' md='3' sm="4" class="px-0" >
            <nuxt-link to="/">
              <v-card-title 
                class="white--text text-decoration-none pa-0"
              >
                AMAZON
              </v-card-title>
            </nuxt-link>
              
          </v-col>
          <v-col cols="12" lg='1' md='3' sm="4" class="px-0" @click="chooseLocationDialog = true">
            <v-card-subtitle class="grey--text subtitle-2 pb-0 ml-5">Hello</v-card-subtitle>
            <v-card-text class="font-weight-bold mt-0 pt-0">
              <v-icon small>mdi-google-maps</v-icon>
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
            <v-button icon  @click="$router.push('/cart')">
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
      class="white black--text"
    >
      <MainMenu />
    </v-navigation-drawer>
    <!-- CHOOSE LOCATION DIALOG --> 
    <v-dialog 
      max-width="500" 
      v-model="chooseLocationDialog"
    >
      <ChooseLocation 
        @closeLocation="closeLocationDialog()"
      />
    </v-dialog>
  </v-container>
</template>

<script>
import MainMenu from '../navigation/mainMenu'
import ChooseLocation from '../navigation/chooseLocation'
export default {
  components: {
    MainMenu,
    ChooseLocation
  },
  data() {
    return {
      drawer: false,
      chooseLocationDialog: false,

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
  },
  methods: {
    closeLocationDialog(){
      this.chooseLocationDialog = false
    },
  }
}
</script>