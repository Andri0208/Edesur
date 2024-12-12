<script setup>

// Lista de licitaciones con sus títulos y contenido descriptivo
const licitacion = [
    {
        title:'Licitación Pública Internacional NO. EDES-LPI-NG-04-2023',
        contenido: 'Para la compraventa de potencia y energía eléctrica entregada mediante contratos de largo plazo de las empresas distribuidoras de electricidad.'
    },
    {
        title: 'Licitación Pública Internacional NO. EDES-LPI-NG-01-2021',
        contenido:'Para la compraventa de potencia y energía eléctrica asociada mediante contratos de largo plazo de las empresas distribuidoras de electricidad EDES.'
    }
]

// Objeto que contiene la ruta de la imagen utilizada en las licitaciones
const img = {
    document: 'public/document-svg.svg fill.png' 
}

</script>

<template>
    <div class="container licitacion">
        <!-- Título principal de la sección de licitaciones -->
        <div class="title-licitacion text-center">
            <h2>Licitación Nacional e Internacional</h2>
        </div>
        
        <div class="container">
            <div class="row">
                <!-- Iteración sobre la lista de licitaciones para generar tarjetas dinámicamente -->
                <div v-for="licitacion in licitacion" class="col col-xl-12 col-mb-2 columna">
                    <div class="card">
                        <div class="card-body">
                            <div class="container text-center">
                                <div class="row">
                                    <!-- Columna para la imagen representativa de cada licitación -->
                                    <div class="col-xl-2">
                                        <img class="img-fluid" :src="img.document" alt="">
                                    </div>
                                    <!-- Columna para el título y contenido de la licitación -->
                                    <div class="col-xl-8">
                                        <h5>{{ licitacion.title }}</h5>
                                        <p>{{ licitacion.contenido }}</p>
                                    </div>
                                    <!-- Columna para el botón de acción "Ver Documento" -->
                                    <div class="col-xl-2 d-flex align-items-center">
                                        <button>
                                            Ver Documento
                                        </button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style>

</style>
