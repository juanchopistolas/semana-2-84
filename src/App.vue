<template>
  <div id="app">
   
    <carousel></carousel>
    <!-- seccion api -->
    <hr color="#ccd1d1" size=3>
    <h5 class = "text-center text-primary font-weight-bold" >SECCIÓN DE NOTICIAS</h5>
    <hr color="#ccd1d1" size=3>
    <sectionapi></sectionapi>
    <!-- fin seccion api -->
  <div class="container-fluid">
  <div class="row justify-content-center mb-5">
    <div class="col mt-5" v-for="(item, index) of member" :key="index">
      <team-card v-bind:member="item">
      </team-card>
    </div>
  </div> 
  <page-footer></page-footer>  
  </div>
  </div>
</template>

<script>
import Carousel from './components/carousel.vue'
import PageFooter from './components/PageFooter.vue'
import TeamCard from './components/TeamCard.vue'
import sectionapi from './components/sectionapi.vue'


export default {
  name: 'App',
  components:{
    Carousel,
    sectionapi,
    PageFooter,
    TeamCard,
  },
  data(){
    return {
      member: [
        {
          codigo: 1,
          Nombre: "Juan Esteban Martinez Arias",
          Descripcion:
            "Tengo 20 años, me encuentro estudiante y me encanta estudiar, dormir y jugar video juegos",
          Rol: "Developer team",
          imagen : "https://github.com/juanchopistolas/semana-2-84/blob/master/src/assets/img/juane.jpg?raw=true",
        },
        {
          codigo: 2,
          Nombre: "Karina Osorio Restrepo",
          Descripcion:
            "Tengo 22 años, me encuentro estudiante y me gusta dormir, comer y pasear",
          Rol: "Developer team",
          imagen: "https://github.com/juanchopistolas/semana-2-84/blob/master/src/assets/img/karina.jpg?raw=true",
        },      
        {
          codigo: 3,
          Nombre: "Carlos Javier Chavarro Parra",
          Descripcion:
            "Tengo 30 años, me encuentro trabajando actualmente y en mi tiempo libro me dedico al  ciclismo",
          Rol: "Developer team",
          imagen : "https://github.com/juanchopistolas/semana-2-84/blob/master/src/assets/img/carlos.jpg?raw=true",
        },
        {
          codigo: 4,
          Nombre: "Cristhian Andrés García Tabares",
          Descripcion:
            "Tengo 21 años, actualmente estudio y me fascina programar",
          Rol: "Developer team",
          imagen : "https://github.com/juanchopistolas/semana-2-84/blob/master/src/assets/img/cristhian.jpg?raw=true",
        },
        {
          codigo: 5,
          Nombre: "Andres Felipe Guerrero Guio",
          Descripcion:
            "Tengo 23 años, me encuentro estudiante y en  mi tiempo libre hago ejercicio",
          Rol: "Scrum Master",
          imagen : "https://github.com/juanchopistolas/semana-2-84/blob/master/src/assets/img/andres.jpg?raw=true",
        },
      ]
    }
  }

}
</script>