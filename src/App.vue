<template>
  <div id="app">
    <section>
      <!-- header -->
      <Header/>

      <!-- main -->
      <Jumbotron/>
      <CurrentSeries/>
      <Services/>
      
      <!-- footer -->
      <Footer/>
      <Subfooter/>
    </section>
    
    
  </div>
</template>

<script>
// importazione componente
import Header from '@/components/Header.vue'
import Jumbotron from '@/components/Jumbotron.vue'
import CurrentSeries from '@/components/CurrentSeries.vue'
import Services from '@/components/Services.vue'
import Footer from '@/components/Footer.vue'
import Subfooter from '@/components/Subfooter.vue'


export default {
  name: 'App',
  // oggetto componenti
  components: {
     Header,
     Jumbotron,
     CurrentSeries,
     Services,
     Footer,
     Subfooter,
  }
}
</script>

<style lang="scss">
// importo stili  @import / @use
@import "./style/general";
@import "./style/utilities";






</style>
