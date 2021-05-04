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

<style lang="scss">

</style>
