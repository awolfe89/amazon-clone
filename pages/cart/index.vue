<template>
  <v-card flat width="100%" class="background">
    <v-row>
      <v-col cols="12" lg='8'>
        <EmptyCart class="mt-10" />
        <v-row class="white mt-7 mx-1">
          <h1 class="my-5">hi</h1>
        </v-row>
        <v-card-subtitle class="subtitle-2 black--text">
          The price and availability of items at Amazon.com are subject to change. The Cart is a temporary place to store a list of your items and reflects each item's most recent price. Shopping Cart
          <span class="ablue--text">Learn more</span>
          
          Do you have a gift card or promotional code? We'll ask you to enter your claim code when it's time to pay.
        </v-card-subtitle>
      </v-col>
      <v-col cols="12" lg='4'>
        <CustomersWhoBought />
      </v-col>
    </v-row>
    <v-row class="mx-5" no-gutters>
      <v-col cols="12">
        <BestSellers class="mt-10" />
      </v-col>
      
    </v-row>
  </v-card>
</template>

<script>
import BestSellers from '../../components/home/bestsellersIn'
import CustomersWhoBought from '../../components/cart/customersWhoBought'
import EmptyCart from '../../components/cart/emptyCart'
export default {
  components: {
    BestSellers,
    CustomersWhoBought,
    EmptyCart,
  },
  data() {
    return {

    }
  }
}
</script>