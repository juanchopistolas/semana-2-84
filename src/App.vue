<template>
  <div id="app">
   
    <carousel></carousel>
    <!-- seccion api -->
    <hr color="#ccd1d1" size=3>
    <h5 class = "text-center text-danger font-weight-bold " >SECCIÓN DE NOTICIAS</h5>
    <hr color="#ccd1d1" size=3>
    <sectionapi></sectionapi>
    <!-- fin seccion api -->
    <page-footer></page-footer>
    
    
  </div>
</template>

<script>
import Carousel from './components/carousel.vue'
import PageFooter from './components/PageFooter.vue'
import sectionapi from './components/sectionapi.vue'



export default {
  name: 'App',
  components:{
    Carousel,
    sectionapi,
    PageFooter,
  }
}
</script>

