<template>
  <div id="app">
    <carousel></carousel>
    <page-footer></page-footer>
    
  </div>
</template>

<script>
import Carousel from './components/carousel.vue'
import PageFooter from './components/PageFooter.vue'



export default {
  name: 'App',
  components:{
    Carousel,
    PageFooter
  }
}
</script>

