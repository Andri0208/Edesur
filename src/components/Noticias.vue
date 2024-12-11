<script setup>
import { computed } from 'vue';


const fondo = [
    {
        fondo: 'public/portada-6.jpg.png',
        fecha:' 29 NOVIEMBRE, 2024',
        contenido:'Edesur Dominicana informa restablecimiento de servicio en centro educativo de Barahona'
    },
    {
        fecha: '29 NOVIEMBRE, 2024',
        contenido: 'Edesur electrifica e ilumina Feria Ecoturística y de Producción en Neiba'
    },
    {
        fondo: 'public/portada-7.jpg.png',
        fecha: ' 26 NOVIEMBRE, 2024',
        contenido:'Edesur instalará dos nuevos transformadores de potencia para mejorar servicio en más de 40 sectores del Distrito Nacional'
    },
    {
        fecha: ' 20 NOVIEMBRE, 2024',
        contenido: 'CUED impulsa inversiones sustanciales para fortalecer la red eléctrica y combatir el fraude energético'
    }
]


</script>

<template>

    <div class="container noticias" >
        <div class="text-center portada-titles">
        <h2>Noticias</h2>
        </div>
        <div class="container ">
  <div class="row align-items-start ">
    <div  v-for="fondo in fondo"
    :key="index" class="col-sm-12 col-md-8 col-lg-6 mb-4 d-flex justify-content-center">
        <div
      :style="{ backgroundImage: `url(${fondo.fondo})`, style }"
      class="portada-noticias"
    >
    <div class="fondo-portada">
        <div class="d-flex justify-content-between  noticias-header">
          <p class="header-parrafo">Comunicacion y Medios</p>
          <p> 29 NOVIEMBRE, 2024</p>  
        </div>
        <div class="noticias-main">
            <p>Edesur Dominicana informa restablecimiento de
                servicio en centro educativo de Barahona</p>
        </div>

        
        <button >
            Mas Informacion >
        </button>
        
        
    </div>
    
    </div>
      
    </div>
  </div>
  <div class="portada-titles d-flex justify-content-center">
  <button>
    Ver mas noticias
  </button>
  </div>
</div>
    </div>

</template>

<style>
</style>