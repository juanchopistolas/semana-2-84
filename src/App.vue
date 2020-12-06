<template>
  <div id="app">
    <carousel></carousel>
    <page-footer></page-footer>
  <div class="container-fluid">
  <div class="row justify-content-center mb-5">
    <div class="col mt-5" v-for="(item, index) of member" :key="index">
      <team-card v-bind:member="item">
      </team-card>
    </div>
  </div>    
  </div>
  </div>
</template>

<script>
import Carousel from './components/carousel.vue'
import PageFooter from './components/PageFooter.vue'
import TeamCard from './components/TeamCard.vue'


export default {
  name: 'App',
  components:{
    Carousel,
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
          Imagen : "../assets/img/juane.jpg",
        },
        {
          codigo: 2,
          Nombre: "Karina Osorio Restrepo",
          Descripcion:
            "Tengo 22 años, me encuentro estudiante y me gusta dormir, comer y pasear",
          Rol: "Developer team",
          Imagen: "../assets/img/karina.jpg",
        },      
        {
          codigo: 3,
          Nombre: "Carlos Javier Chavarro Parra",
          Descripcion:
            "Tengo 30 años, me encuentro trabajando actualmente y en mi tiempo libro me dedico al  ciclismo",
          Rol: "Developer team",
          Imagen : "../assets/img/carlos.jpg",
        },
        {
          codigo: 4,
          Nombre: "Cristhian Andrés García Tabares",
          Descripcion:
            "Tengo 21 años, actualmente estudio y me fascina programar",
          Rol: "Developer team",
          Imagen : "../assets/img/cristhian.jpg",
        },
        {
          codigo: 5,
          Nombre: "Andres Felipe Guerrero Guio",
          Descripcion:
            "Tengo 23 años, me encuentro estudiante y en  mi tiempo libre hago ejercicio",
          Rol: "Scrum Master",
          Imagen : "../assets/img/andres.jpg",
        },
      ]
    }
  }

}
</script>