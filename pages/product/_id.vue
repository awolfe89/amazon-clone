<template>
  <v-container fluid class="white">
    <AdBar />
    <v-row>
      <v-breadcrumbs :items="breadcrumbs" />
    </v-row>
    
    <v-row>
      <!-- IMAGE --> 
      <v-col cols="12" lg="3">
        <v-img
          src="https://picsum.photos/510/300?random"
          aspect-ratio="1.7"
        />
      </v-col>
      <!-- TEXT --> 
      <v-col cols="12" lg='6'>
        <R2Column />
      </v-col>
      <!-- PRICING / CART --> 
      <v-col cols="12" lg="3">
        <R3Column />
      </v-col>
    </v-row>
    <v-divider class="background" />
    
    <BuyWith />

    <FourStarsAndAbove />

    <RelatedProducts />


    <AlsoViewed />
    <Recommended />
    <UltimatelyBought />

    <SignInRow />
  </v-container>
</template>

<script>
import AdBar from '../../components/navigation/productAdBar'
import R2Column from '../../components/product/r2Column'
import R3Column from '../../components/product/r3Column'
import BuyWith from '../../components/product/buyWith'
import FourStarsAndAbove from '../../components/product/fourStarsAndAbove'
import RelatedProducts from '../../components/product/relatedProducts'
import AlsoViewed from '../../components/product/alsoViewed'
import Recommended from '../../components/product/recommendedBasedTrends'
import UltimatelyBought from '../../components/product/ultimatelyBought'
import SignInRow from '../../components/home/signInRow'

export default {
 components: {
   AdBar,
   R2Column,
   R3Column,
   BuyWith,
   FourStarsAndAbove,
   RelatedProducts,
   AlsoViewed,
   Recommended,
   UltimatelyBought,
   SignInRow
 }, 
 data() {
   return {
     breadcrumbs: [
      {
        text: 'Home',
        disabled: false,
        href: '/',
      },
      {
        text: 'blah',
        disabled: false,
        href: '/#/administrative',
      },
      {
        text: 'blah',
        disabled: true,
      },
    ],
   }
 }
}
</script>