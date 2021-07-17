<template>
  <div id="app">
      <Header :items= "items"/>
      <Main/>
      <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
      Header,
      Main,
      Footer
  },
  data() {
      return{
        items: [
      {message: 'Home'},
      {message: 'Mission'},
      {message: 'Causes'},
      {message: 'Journal'}
    ],
        
      }
  }
}
</script>

<style lang="scss">
  @import '@/style/commons.scss'
</style>
