<template>
  <v-card width="100%" flat class="background">
    <Slider />
    <TopBlock />
    <DvdSlider />
    <MadeInItalySlider />
    <FourCategoryBlock />
    <TrendingDeals />
    <Livestream />
    <FrequentlyPurchased />
    <Banner />
    <SecondFourCategory />
    <BestsellersIn />
    <Slider6 />
    <Bottom4Block />
    <Slider7 />
    <Slider8 />
    <SignInRow />

  </v-card>
</template>

<script>
import Slider from '../components/home/slider'
import TopBlock from '../components/home/topBlock'
import DvdSlider from '../components/home/dvdSlider'
import MadeInItalySlider from '../components/home/madeInItalySlider'
import FourCategoryBlock from '../components/home/fourCategoryBlock'
import TrendingDeals from '../components/home/trendingDeals'
import Livestream from '../components/home/livestream'
import FrequentlyPurchased from '../components/home/frequentlyPurchased'
import SecondFourCategory from '../components/home/secondFourCategory'
import BestsellersIn from '../components/home/bestsellersIn'
import Banner from '../components/home/banner'
import Slider6 from '../components/home/slider6'
import Bottom4Block from '../components/home/bottom4Block'
import Slider7 from '../components/home/slider7'
import Slider8 from '../components/home/slider8'
import SignInRow from '../components/home/signInRow'
export default {
  name: 'IndexPage',
  components: {
    Slider,
    TopBlock,
    DvdSlider,
    MadeInItalySlider,
    FourCategoryBlock,
    TrendingDeals,
    Livestream,
    FrequentlyPurchased,
    SecondFourCategory,
    BestsellersIn,
    Banner,
    Slider6,
    Bottom4Block,
    Slider7,
    Slider8,
    SignInRow
  },
  data() {
    return {

    }
  }
}
</script>
