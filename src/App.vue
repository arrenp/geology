<template>
<div class="d-flex flex-column justify-content-between" style="overflow:hiddden">
  <Header />
  <Body/>
  <Footer /> 
</div>
  
</template>

<script>
import Header from './components/mainApp/Header.vue';
import Body from './components/mainApp/Body.vue';
import Footer from './components/mainApp/Footer.vue';
export default {
  name: 'App',
  components: {
    Header,
    Body,
    Footer
  },
  methods:{
    handleScroll() {
        console.log('scrolled')
      }
    }
  
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
