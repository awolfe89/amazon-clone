<template>
  <v-app>
    <TopBar /> 
    
    <v-main>
      <v-container class="background" fluid>
        <Nuxt />
      </v-container>
    </v-main>
    
    <Footer1 />
    <Footer2 />
    <Footer />
  </v-app>
</template>

<script>
import TopBar from '../components/navigation/topBar.vue'
import Footer from '../components/navigation/footer.vue'
import Footer1 from '../components/navigation/footer1'
import Footer2 from '../components/navigation/footer2'
export default {
  name: 'DefaultLayout',
  components :{
    TopBar,
    Footer,
    Footer1,
    Footer2,
  },
  data () {
    return {
      drawer: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],

      title: 'Vuetify.js'
    }
  }
}
</script>
