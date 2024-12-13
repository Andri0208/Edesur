<script setup>
// Lista de certificaciones con sus imágenes y descripciones
const certificaciones = [
    {
        img: 'public/Background+Border-1.png',
        contenido: 'Sistema de Gestión de Compliance No. Registro R20210903-01'
    },
    {
        img: 'public/Background+Border-2.png',
        contenido: 'Sistema de Gestión de Antisoborno No. Registro R20210903-02'
    },
    {
        img: 'public/Background+Border-3.png',
        contenido: 'Sistema de Gestión de la Calidad No. Registro R20210903-03'
    }
]

</script>

<template>
<div class="container base">
    <!-- Sección principal de certificaciones -->
    <div class="certificaciones">
        <!-- Título principal de la sección -->
        <div class="certificaciones-title text-center">
            <h3>Certificaciones Internacionales del Sistema de Gestión de la <br> <span>Calidad, Cumplimiento y Antisoborno</span></h3>
        </div>
        <!-- Descripción general de las certificaciones -->
        <div class="contenido-title text-center">
            <p>
                Certificaciones que avalan el cumplimiento de los diferentes estándares internacionales producidos y promovidos por la Organización Internacional de Normalización (ISO).
            </p>
        </div>

        <div class="container text-center">
            <div class="row">
                <!-- Iteración sobre la lista de certificaciones para generar elementos dinámicos -->
                <div v-for="certificaciones in certificaciones" class="col col-xl-4">
                    <!-- Imagen de cada certificación -->
                    <div>
                        <img :src="certificaciones.img" alt="">
                    </div>
                    <!-- Descripción de cada certificación -->
                    <div>
                        <p>{{ certificaciones.contenido }}</p>
                    </div>
                </div>
            </div>
        </div>

    </div>
</div>

</template>

<style>

</style>
