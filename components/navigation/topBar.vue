<template>
  <v-container fluid>
    <v-row class="py-2 dark" >
      <v-app-bar flat class="dark py-2 my-2">
          <v-col cols="2" class="px-0">
              <v-toolbar-title class="px-0">AMAZON</v-toolbar-title>
          </v-col>
          <v-col cols="2" class="px-0">
            <v-card-text class="font-weight-bold">
              <v-icon>mdi-google-maps</v-icon>
              Select Your Address
            </v-card-text>
          </v-col>
          <v-col cols="4">
            <v-text-field 
              outlined 
              placeholder="search" 
              prepend-inner-icon="mdi-magnify"
              class="mt-2"
              />
          </v-col>
          <v-col cols="2">
            <v-card-text class="my-0 py-0">Hello, sign in</v-card-text>
            <v-card-text class="my-0 py-0 font-weight-bold">Account & Lists</v-card-text>
          </v-col>
          <v-col cols="2">
            <v-button icon>
              <v-icon color="warning" large>mdi-cart-outline</v-icon>
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

    <!-- NAV DRAWER --> 
    <v-navigation-drawer
      v-model="drawer"
      app
      temporary
      clipped-left="clipped"

    >
      <v-row class="primary my-1">
        <v-card-title class="">
          <v-icon large class="mr-1">mdi-account-circle</v-icon>
          Hello, Sign In
        </v-card-title>
      </v-row>
      <v-list>
        <v-list-item>
          <v-list-item-content>
            <v-list-item-title class="text-h6">
              Trending
            </v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item>
          <v-list-item-content>
            Bestsellers
          </v-list-item-content>
        </v-list-item>
        <v-list-item>
          <v-list-item-content>
            New Releases
          </v-list-item-content>
        </v-list-item>
        <v-list-item>
          <v-list-item-content>
            Movers & Shakers
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <v-list>
        <v-list-item>
          <v-list-item-content>
            <v-list-item-title class="text-h6">
              Digital Content & Devices
            </v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      <v-list-group
        v-for="item in items"
        :key="item.title"
        v-model="item.active"
        :prepend-icon="item.action"
        no-action
      >
        <template v-slot:activator>
          <v-list-item-content>
            <v-list-item-title v-text="item.title"></v-list-item-title>
          </v-list-item-content>
        </template>

        <v-list-item
          v-for="child in item.items"
          :key="child.title"
        >
          <v-list-item-content>
            <v-list-item-title v-text="child.title"></v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list-group>
    </v-list>
    </v-navigation-drawer>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      drawer: true,
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
      ],
       items: [
        {
          action: 'mdi-ticket',
          items: [{ title: 'List Item' }],
          title: 'Attractions',
        },
        {
          action: 'mdi-silverware-fork-knife',
          active: true,
          items: [
            { title: 'Breakfast & brunch' },
            { title: 'New American' },
            { title: 'Sushi' },
          ],
          title: 'Dining',
        },
        {
          action: 'mdi-school',
          items: [{ title: 'List Item' }],
          title: 'Education',
        },
        {
          action: 'mdi-human-male-female-child',
          items: [{ title: 'List Item' }],
          title: 'Family',
        },
        {
          action: 'mdi-bottle-tonic-plus',
          items: [{ title: 'List Item' }],
          title: 'Health',
        },
        {
          action: 'mdi-briefcase',
          items: [{ title: 'List Item' }],
          title: 'Office',
        },
        {
          action: 'mdi-tag',
          items: [{ title: 'List Item' }],
          title: 'Promotions',
        },
      ],
    }
  }
}
</script>