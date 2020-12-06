<template>
    <div class="card text-white bg-dark" id= "team" >
        <div class="card-body m-3">
        <div class="d-flex justify-content-center">
            <img :src="member.imagen" width="160px" height="250px" alt="Fotografia del Integrante">
        </div>
            <p class="card-text">{{member.Rol}}</p>            
            <h5 class="card-title">{{member.Nombre}}</h5>
            <p class="card-text">{{member.Descripcion}}</p>
        </div>
    </div>
</template>

<script>
    export default {
        name: "TeamCard",
        props: ['member']
    }
</script>

<style scoped>

</style>