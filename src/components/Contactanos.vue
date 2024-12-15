<script setup>
const img = {
    img1: 'public/24-hours-support.svg fill.png',
    img2: 'public/messange-box.svg fill.png',
    img3: 'public/banner-web-2.png.png'
}


</script>

<template>
<div class="container contactanos">
    <div class="container text-center">
  <div class="row align-items-center">
    <div class="col " >
      <h2>Contáctanos las 24 horas, los
        365 días del año.</h2>
        <p>Comunícate a nuestro Centro de Atención Telefónica para recibir asistencia personalizada.</p>
        <div class="row atencion">
            <div class="col-6">
                <div class="d-flex text-center">
                    <div>
                    <img :src="img.img1" alt="">
                    </div>
                    <div class="cell">
                    <h5>Call Center</h5>
                    <p>809-683-9393</p>
                    </div>
                </div>
            </div>
            <div class="col-6">
                <div class="d-flex text-center">
                    <div>
                    <img :src="img.img2" alt="">
                    </div>
                    <div class="cell">
                    <h5>Chat Bot</h5>
                    <p>809-683-9393</p>
                    </div>
                </div>
            </div>

        </div>
    </div>
    <div class="col">
        <img :src="img.img3" class="img-fluid" alt="...">
    </div>
  </div>
</div>

</div>

</template>

<style>

</style>