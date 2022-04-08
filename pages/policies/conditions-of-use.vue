<template>
  <v-container fluid>
    <v-card-title class="display-1 black--text">
      Help & Customer Service
    </v-card-title>
    
    <v-row>
      <v-col cols="12" lg='3' class="px-0">
        <v-card class="white" flat width="100%">
          <v-card-text class="black--text">
            Legal Policies
          </v-card-text>

          <v-card-subtitle class="black--text pb-0">
            3rd Party Licensing Notice (Mobile App)
          </v-card-subtitle>
          <v-card-subtitle class="black--text font-weight-bold py-1">
            Conditions of Use
          </v-card-subtitle>
          <v-card-subtitle class="black--text py-1">
            Amazon.com privacy notice
          </v-card-subtitle>
          <v-card-subtitle class="black--text py-1">
            Amazon group companies
          </v-card-subtitle>
          <v-card-subtitle class="black--text py-1">
            Amazon trademark useage guidelines
          </v-card-subtitle>
          <v-card-subtitle class="black--text py-1">
            non-exhaustive list of Amazon trademarks
          </v-card-subtitle>
          <v-card-subtitle class="black--text pt-0 pb-6">
            Amazon.com gift card and electronic message customization service terms
          </v-card-subtitle>
        </v-card> 

        <v-card class="white mt-4">
          <v-card-text class="black--text">
            Quick Solutions
          </v-card-text>
          <v-row v-for="menuItem in menuItems" :key="menuItem">
            <v-col cols="12" lg="4" class="d-flex justify-center pr-0">
              <v-icon color='black' large>{{menuItem.icon}}</v-icon>
            </v-col>
            <v-col cols="12" lg="8" class="ml-0 pl-0">
              <v-card-text class="black--text font-weight-bold py-0">{{ menuItem.title}}</v-card-text>
              <v-card-subtitle class="black--text py-0">{{menuItem.subtitle}}</v-card-subtitle>
            </v-col>
          </v-row>
        </v-card>
      </v-col>
      <v-col cols="12" lg='6'>
        <v-card class="white" flat>
          <v-card-title class="black--text">
            Find more solutions
          </v-card-title>
          <v-text-field solo light append-icon="mdi-magnify" class="mx-4" />
          <v-card-title class="black--text font-weight-bold">Conditions of Use</v-card-title>
          <v-card-subtitle class="black--text font-weight-bold">Last updated: May 3, 2021</v-card-subtitle>
          <v-card-text class="black--text">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus, cum enim architecto iure distinctio accusantium quae error similique hic minus voluptates. Minus suscipit temporibus repudiandae debitis nostrum tempora vel dolorem.
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi numquam laudantium, incidunt totam est eius expedita at esse voluptatum nihil quo hic dolore ducimus asperiores velit necessitatibus molestiae, debitis mollitia.
          </v-card-text>
          <v-card-text class="black--text">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus, cum enim architecto iure distinctio accusantium quae error similique hic minus voluptates. Minus suscipit temporibus repudiandae debitis nostrum tempora vel dolorem.
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Error molestias sit voluptatum, odio possimus fugiat nam labore unde at ex ipsa quae iure voluptatibus necessitatibus quam aut minima dolorum non!
          </v-card-text>
          <v-card-text class="black--text">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus, cum enim architecto iure distinctio accusantium quae error similique hic minus voluptates. Minus suscipit temporibus repudiandae debitis nostrum tempora vel dolorem.
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>

  </v-container>
</template>

<script>
export default {
  data(){ 
    return {
      menuItems: [
        {
          icon: 'mdi-package',
          title: 'Your Orders',
          subtitle: 'Track or Cancel Orders'
        },
        {
          icon: 'mdi-package-variant',
          title: 'Returns & Refunds',
          subtitle: 'Exchange or Return Items'
        },
        {
          icon: 'mdi-amazon',
          title: 'Manage Prime',
          subtitle: 'Cancel or view benefits'
        },
        {
          icon: 'mdi-credit-card',
          title: 'Payment Settings',
          subtitle: 'Track or Cancel Orders'
        },
        {
          icon: 'mdi-truck',
          title: 'Carrier Info',
          subtitle: 'Shipping Carrier Information'
        },
        {
          icon: 'mdi-account-circle-outline',
          title: 'Account Settings',
          subtitle: 'Change email or password'
        },
      ]
    }
  }
}
</script>