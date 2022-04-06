<template>
<v-card width="100%" class="secondary">
    <v-row class="d-flex justify-space-between my-10">
    <v-col cols="12" lg="3" class="d-flex justify-center">
      <v-card width="100%" class="mx-2 secondary" flat>
        <v-card-title class="d-flex justify-center">Get To Know Us</v-card-title>
        <v-card-text class="d-flex justify-center my-0 py-0 white--text" v-for="getLink in GetToKnowUs" :key="getLink">
         {{ getLink }}
         </v-card-text>
      </v-card>
    </v-col>

    <v-col cols="12" lg="3" class="d-flex justify-center">
      <v-card width="100%" class="mx-2 secondary" flat>
        <v-card-title class="d-flex justify-center">Make Money With Us</v-card-title>
        <v-card-text class="d-flex justify-center my-0 py-0 white--text" v-for="moneyLink in MakeMoneyWithUs" :key="moneyLink">
         {{ moneyLink }}
         </v-card-text>
      </v-card>
    </v-col>
    <v-col cols="12" lg="3" class="d-flex justify-center">
      <v-card width="100%" class="mx-2 secondary" flat>
        <v-card-title class="d-flex justify-center">Amazon Payment Products</v-card-title>
        <v-card-text class="d-flex justify-center my-0 py-0 white--text" v-for="paymentLink in AmazonPaymentProducts" :key="paymentLink">
         {{ paymentLink }}
         </v-card-text>
      </v-card>
    </v-col>
    <v-col cols="12" lg="3" class="d-flex justify-center">
      <v-card width="100%" class="mx-2 secondary" flat>
        <v-card-title class="d-flex justify-center">Amazon Payment Products</v-card-title>
        <v-card-text class="d-flex justify-center my-0 py-0 white--text" v-for="helpLink in LetUsHelpYou" :key="helpLink">
         {{ helpLink }}
         </v-card-text>
      </v-card>
    </v-col>>
  </v-row>
</v-card>

</template>

<script>
export default {
  data() {
    return {
      GetToKnowUs: ["Careers", "Blog", "About Amazon", "Sustainability", "Press Center", "Investor Relations","Amazon Devices", "Amazon Science",],
      MakeMoneyWithUs: ["Sell Products on Amazon", "Sell Apps on Amazon", "Become an Affiliate", "Become a Delivery Driver", "Start a Package Delivery Business", "Advertise Your Products", "Self-Publish with Us", "Host an Amazon Hub", "See More Ways to Make Money",],
      AmazonPaymentProducts: ["Amazon Rewards Visa Signature Cards", "Amazon Store Card", "Amazon Secured Card", "Amazon Business Card", "Amazon Business Line of Credit", "Shop with Points", "Credit Card Marketplace", "Reload Your Balance", "Amazon Currency Converter",],
      LetUsHelpYou: ["Amazon and COVID-19", "Your Account", "Your Orders", "Shipping Rates & Policies", "Amazon Prime", "Returns & Replacements", "Manage Your Content and Devices", "Amazon Assistant", "Help",],
    }
  }
}
</script>