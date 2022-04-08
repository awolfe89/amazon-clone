<template>
  <v-card class="white" flat>
      <v-row class="primary my-1 mt-0 pt-0">
        <v-card-title class="">
          <v-icon large class="mr-1">mdi-account-circle</v-icon>
          Hello, Sign In
        </v-card-title>
        
      </v-row>
      <v-row v-for="menuItem in menu" :key="menuItem"  >
        <v-card-title 
          class="h6-text black--text"
          
        >
          {{menuItem.title}}
        </v-card-title>
        <v-card-text
          class="black--text"
          v-for="item in menuItem.subItem" :key="item"
        >
          {{ item.title }}
        </v-card-text>
      </v-row>
  </v-card>
</template>

<script>
  export default {
    data: () => ({
      menu: [
        { title: 'Trending',
          subItem: [{title: 'hi'}, {title: 'mre'}],
        },
        { title: 'Digital Content & Devices',
          subItem: [{title: 'hi'}, {title: 'mre'}]
        },
        { title: 'Shop By Department',
          
        },
        { title: 'Programs & Features',
          
        },
        { title: 'Help & Settings',
          
        },
      ]
    }),
  }
</script>