<template>
  <div id="app">
      <Header :items= "items"/>
      <Main/>
      <Footer :socialIcons= "socialIcons"/>
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
      socialIcons: [
        '<i class="fab fa-facebook-f"></i>',
        '<i class="fab fa-instagram"></i>',
        '<i class="fab fa-twitter"></i>',
        '<i class="fab fa-youtube"></i>'
      ]
        
      }
  }
}
</script>

<style lang="scss">
  @import '@/style/commons.scss'
</style>
