<template>
  <div id="app">
    <section>
      <!-- header -->
      <Header/>

      <!-- main -->
      <Main/>
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
import Main from '@/components/Main.vue'
import Services from '@/components/Services.vue'
import Footer from '@/components/Footer.vue'
import Subfooter from '@/components/Subfooter.vue'


export default {
  name: 'App',
  // oggetto componenti
  components: {
     Header,
     Main,
     Services,
     Footer,
     Subfooter,
  }
}
</script>

<style>

/* GENERAL */

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container{
  max-width: 1200px;
  margin: 0 auto;
  font-family: sans-serif;
}


/* UTILITIES */
.flex{
  display: flex;
}

.grow{
  flex-grow: 1;
  justify-content: flex-end;
}




</style>
