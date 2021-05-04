<template>
  <div id="app">
    <section>
      <!-- header -->
      <Header/>

      <!-- main -->
      <Main/>

      <!-- footer -->
      <footer>footer</footer>
    </section>
    
    
  </div>
</template>

<script>
// importazione componente
import Header from '@/components/Header.vue'
import Main from '@/components/Main.vue'


export default {
  name: 'App',
  // oggetto componenti
  components: {
     Header,
     Main,
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




</style>
