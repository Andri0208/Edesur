<script setup>
const informacionAlCliente = [
    {
        img: 'public/informacionAlCliente/iconos-para-pagina-web-edesur_tarifa-ele-ctrica.svg fill.png',
        title: 'Puntos de Pago',
        contenido: 'Localiza nuestras oficinas o estafetas mas cercanas.', 
    },
    {
        img: 'public/informacionAlCliente/iconos-para-pagina-web-edesur_tarifa-ele-ctrica.svg fill.png',
        title: 'Tarifa Electrica',
        contenido: 'Lista de los precios de energía por ano.', 
    },
    {
        img: 'public/informacionAlCliente/iconos-para-pagina-web-edesur_tarifa-ele-ctrica.svg fill.png',
        title: 'Mantenimientos Programados',
        contenido: 'Verifica los Mantenimientos Programados de la Semana.', 
    },
    {
        img: 'public/informacionAlCliente/iconos-para-pagina-web-edesur_tarifa-ele-ctrica.svg fill.png',
        title: 'Cambio de Titular',
        contenido: 'Cambio de Titular de persona Física a Empresa.', 
    },
    {
        img: 'public/informacionAlCliente/iconos-para-pagina-web-edesur_tarifa-ele-ctrica.svg fill.png',
        title: 'Informacion Ciudadana PIC',
        contenido: 'Información de mejoras en la distribución eléctrica de Edesur.', 
    },

]

</script>

<template>
    <section>

<div id="informacion-al-cliente-title">
    <h1>Información al Cliente</h1>
</div>

<div class="informacion-al-cliente">
    <div class="container text-center">
  <div class="row align-items-start">
    <div v-for="informacionAlCliente in informacionAlCliente" class="col-12 col-sm-4 mt-4  " >
        <div class=" card " id="card-informacion-al-cliente">
            <div class="card-cliente d-flex align-items-center">
      <a href="#" class="nav-link">
        <div class="row g-0">
             <div class="col-2">
                <img :src="informacionAlCliente.img" alt="">
            </div>
            <div class="col-10">
                <h5>{{ informacionAlCliente.title }}</h5>
                <p>{{ informacionAlCliente.contenido }}</p>
            </div>
        </div>
      </a>
      </div>
      </div>

      </div>
    </div>
    
  </div>
</div>


</section>

</template>

<style>


</style>