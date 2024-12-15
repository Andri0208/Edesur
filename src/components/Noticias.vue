<script setup>
// Importación del método computed desde Vue
import { computed } from 'vue';

// Datos de noticias con información como fondo, fecha y contenido
const fondo = [
    {
        fondo: 'public/portada-6.jpg.png',
        fecha: '29 NOVIEMBRE, 2024',
        contenido: 'Edesur Dominicana informa restablecimiento de servicio en centro educativo de Barahona'
    },
    {
        fecha: '29 NOVIEMBRE, 2024',
        contenido: 'Edesur electrifica e ilumina Feria Ecoturística y de Producción en Neiba'
    },
    {
        fondo: 'public/portada-7.jpg.png',
        fecha: '26 NOVIEMBRE, 2024',
        contenido: 'Edesur instalará dos nuevos transformadores de potencia para mejorar servicio en más de 40 sectores del Distrito Nacional'
    },
    {
        fecha: '20 NOVIEMBRE, 2024',
        contenido: 'CUED impulsa inversiones sustanciales para fortalecer la red eléctrica y combatir el fraude energético'
    }
];
</script>

<template>
    <!-- Contenedor principal para la sección de noticias -->
    <div class="container noticias ">
        <!-- Título de la sección "Noticias" -->
        <div class="text-center portada-titles">
            <h2>Noticias</h2>
        </div>

        <!-- Contenedor para las noticias -->
        <div class="container">
            <div class="row align-items-start">
                <!-- Renderizado dinámico de las noticias con v-for -->
                <div v-for="(item, index) in fondo" :key="index" 
                    class="col-sm-12 col-md-8 col-lg-6 mb-4 d-flex justify-content-center">
                    <!-- Contenedor individual de cada noticia con fondo dinámico -->
                    <div :style="{ backgroundImage: `url(${item.fondo})` }" class="portada-noticias">
                        <div class="fondo-portada">
                            <!-- Encabezado de la noticia con texto alineado -->
                            <div class="d-flex justify-content-between noticias-header">
                                <p class="header-parrafo">Comunicacion y Medios</p>
                                <p>{{ item.fecha }}</p>  
                            </div>
                            <!-- Contenido principal de la noticia -->
                            <div class="noticias-main">
                                <p>{{ item.contenido }}</p>
                            </div>
                            <!-- Botón para ver más información -->
                             <div>
                            <button>Mas Informacion ></button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <!-- Botón para cargar más noticias -->
            <div class="portada-titles d-flex justify-content-center">
                <button>Ver más noticias</button>
            </div>
        </div>
    </div>
</template>

<style>


</style>
