<template>
    <div>
        <div class="card text-white bg-dark">
            <div class="d-flex justify-content-center p-2">
                <img v-bind:src="member.Imagen" alt="Fotografia del miembro">
            </div>
            <div class="card-body">
                <p class="card-text">{{member.Rol}}</p>            
                <h5 class="card-title">{{member.Nombre}}</h5>
                <p class="card-text">{{member.Descripcion}}</p>
            </div>
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