<template>
  <div id="app">
    <page-header></page-header>
    <carousel></carousel>
    <page-footer></page-footer>
    
    
  </div>
</template>

<script>
import Carousel from './components/carousel.vue'
import PageFooter from './components/PageFooter.vue'
import PageHeader from './components/PageHeader.vue'



export default {
  name: 'App',
  components:{
    Carousel,
    PageFooter,
    PageHeader,
  }
}
</script>

