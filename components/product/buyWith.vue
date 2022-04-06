<template>
  <v-card class="white" flat width="100%">
    <v-card-title class="warning--text pb-9">Buy it with</v-card-title>
    <v-row>
      <v-col cols="12" lg='6'>
        <v-row class="mb-0 pb-0">
          <v-col cols="12" lg='3'>
            <v-img
              src="https://picsum.photos/510/300?random"
              aspect-ratio="1.7"
            />
          </v-col>
          <v-col cols="12" lg='3'>
            <v-img
              src="https://picsum.photos/510/300?random"
              aspect-ratio="1.7"
            />
          </v-col>
          <v-col cols="12" lg='3'>
            <v-img
              src="https://picsum.photos/510/300?random"
              aspect-ratio="1.7"
            />
          </v-col>
          <v-col cols="12" lg='3'>
            <v-card-text class="grey--text">Total Price:
              <span class="error--text">$380.37</span>
            </v-card-text>
            <v-btn class="bright black--text" small>Add all three to cart</v-btn>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
    <v-row class="pt-0 mt-0">
      <v-col cols="12" lg='10' >
        <v-card-subtitle class="black--text mt-0 pt-0">
             <v-icon color="ablue">mdi-information</v-icon>
             These items are shipped from and sold by different sellers.
            <span class="ablue--text">Show details</span></v-card-subtitle>
           
             
             <v-checkbox color="blue" v-model="something" class="ml-4 mt-0 pt-0">
               <template v-slot:label>
                  <v-card-text class="black--text my-0 py-0">
                    <span class="font-weight-bold">This item:</span>
                    NGNWOB Rate 3500W / Peak 7000W car RV Truck Solar Inverter Power Inverter DC12V to AC 120V Power C...
                    <span class="error--text">$259.00</span>
                  </v-card-text>
               </template>
             </v-checkbox>
             <v-checkbox color="blue" v-model="something" class="ml-4 my-0 py-0">
               <template v-slot:label>
                  <v-card-text class="black--text my-0 py-0">
                    <span class="font-weight-bold">This item:</span>
                    NGNWOB Rate 3500W / Peak 7000W car RV Truck Solar Inverter Power Inverter DC12V to AC 120V Power C...
                    <span class="error--text">$259.00</span>
                  </v-card-text>
               </template>
             </v-checkbox>
             <v-checkbox color="blue" v-model="something" class="ml-4 my-0 py-0">
               <template v-slot:label>
                  <v-card-text class="black--text my-0 py-0">
                    <span class="font-weight-bold">This item:</span>
                    NGNWOB Rate 3500W / Peak 7000W car RV Truck Solar Inverter Power Inverter DC12V to AC 120V Power C...
                    <span class="error--text">$259.00</span>
                  </v-card-text>
               </template>
             </v-checkbox>
             
      </v-col>
    </v-row>
    <v-divider class="background" />
  </v-card>
</template>

<script>
export default {
  data() {
    return{ 
      something: true,
    }
  }
}
</script>