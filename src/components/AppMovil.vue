<script setup>
const appMovilImg = {
    playStores: 'public/google-badge.svg fill.png',
    appStores: 'public/apple-badge.svg.png',
    iphoneApp:'public/iphone-appmovil@2x.png.png'
} 

</script>

<template>
<div class="app-movil-titles text-center container" >
    <h6>App Movil Edesur</h6>
    <h2>¡Aprovecha al máximo tus servicios!</h2>
    <p>¿Estás buscando una forma rápida y sencilla de gestionar tus servicios eléctricos? No busques más. Con nuestra<br>
        app móvil de Edesur, podrás realizar una amplia gama de acciones con unos pocos toques.</p>
    <div class="d-flex justify-content-center">
        <img :src="appMovilImg.playStores" class="img-fluid" alt="Playstores">
        <img :src="appMovilImg.appStores" class="img-fluid" alt="AppStores">
    </div>
    <div>
        <button class="btn ">
            Mas Informacion 
        </button>
    </div>
    <div class="app-stores">
        <img :src="appMovilImg.iphoneApp" class="img-fluid" alt="">
    </div>

</div>
</template>

<style>


</style>