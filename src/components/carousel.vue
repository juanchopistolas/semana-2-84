<template>
    <!-- carousel -->
    <div id="carouselExampleCaptions" class="carousel slide" data-ride="carousel">
        <ol class="carousel-indicators">
            <li data-target="#carouselExampleCaptions" data-slide-to="0" class="active"></li>
            <li data-target="#carouselExampleCaptions" data-slide-to="1" class=""></li>
            <li data-target="#carouselExampleCaptions" data-slide-to="2" class=""></li>
        </ol>
        <div class="carousel-inner">
            <div class="carousel-item active">
                <img class="bd-placeholder-img bd-placeholder-img-lg d-block w-100" width="800" height="400" src="../assets/img/ConsultorioContable.jpg"  alt="First slide"
                preserveAspectRatio="xMidYMid slice" focusable="false" role="img">
                <div class="carousel-caption d-none d-md-block" >
                    <h4 class="font-weight-bold">Consultorio Contable</h4>
                    <p class="font-weight-bold">Realizamos acompañamiento y desarrollamos procesos necesarios en el área administrativa.
                    <br>Desarrollamos un proceso de alta efectividad contable</p>
                </div>
            </div>
            <div class="carousel-item">
                <img class="bd-placeholder-img bd-placeholder-img-lg d-block w-100" width="800" height="400" src="../assets/img/ConsultorioJuridico.jpg"  alt="First slide"
                preserveAspectRatio="xMidYMid slice" focusable="false" role="img">
                <div class="carousel-caption d-none d-md-block">
                    <h4 class="font-weight-bold">Consultorio jurídico</h4>
                    <p class="font-weight-bold">Ofrecemos servicios jurídicos a personas juridicas, con el objetivo de proveer soluciones efectivas y eficaces a nuestros clientes.</p>
                </div>
            </div>
            <div class="carousel-item">
                <img class="bd-placeholder-img bd-placeholder-img-lg d-block w-100" width="800" height="400" src="../assets/img/DesarrolloWeb.jpg"  alt="First slide"
                preserveAspectRatio="xMidYMid slice" focusable="false" role="img">
                <div class="carousel-caption d-none d-md-block">
                    <h4 class="font-weight-bold">Servicio Desarrollo WEB</h4>
                    <p class="font-weight-bold">Desarrollamos páginas web pensando en el perfil de tu marca y en el futuro de tu empresa.</p>
                </div>
            </div>
        </div>
        <a class="carousel-control-prev" href="#carouselExampleCaptions" role="button" data-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Previous</span>
        </a>
        <a class="carousel-control-next" href="#carouselExampleCaptions" role="button" data-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Next</span>
        </a>
    </div>
</template>

<script>
export default {
    name: 'carousel',
}
</script>

<style scoped>

</style>