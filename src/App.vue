<template>
  <div id="app">
    <section>
      <!-- header -->
      <Header/>

      <!-- main -->
      <main>main</main>

      <!-- footer -->
      <footer>footer</footer>
    </section>
    
    
  </div>
</template>

<script>
// importazione
import Header from '@/components/Header.vue'

export default {
  name: 'App',
  components: {
    // oggetto component
     Header,
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
