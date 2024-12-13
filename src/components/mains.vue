<script setup>
const carrusel = [
  { img: 'public/carrusel-1.png.png' },
  { img: 'public/carrusel-2.png.png' },
  { img: 'public/carrusel-3.png.png' },
  { img: 'public/carrusel-4.png.png' }
];

const card = {
  vector: 'public/card/Vector.png',
  elipse: 'public/card/Elipse 321.png'
};

const cardImg = [
  {
    cardImg: 'public/card/card-1.png',
    Text: 'REPORTE DE AVERIAS'
  },
  {
    cardImg: 'public/card/card-2.png',
    Text: 'RECLAMACIONES'
  },
  {
    cardImg: 'public/card/card-3.png',
    Text: 'PAGO DE SERVICIOS'
  },
  {
    cardImg: 'public/card/card-4.png',
    Text: 'NUEVO CONTRATO'
  },
  {
    cardImg: 'public/card/card-5.png',
    Text: 'CANAL DE DENUNCIAS'
  }
];

const banner = {
  img: 'public/OV-Banner.png.png'
};
</script>

<template>
  <!-- Carrusel -->
  <div id="carouselExample" class="carousel slide">
    <div class="carousel-inner">
      <div 
        v-for="(item, index) in carrusel" 
        :key="index" 
        :class="['carousel-item', { active: index === 0 }]">
        <img :src="item.img" class="d-block w-100" alt="...">
      </div>
    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Previous</span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Next</span>
    </button>
  </div>
  <!-- Fin del carrusel -->

  <!-- Sección de tarjetas -->
  <section id="tarjeta" class="container base">
    <div class="container banner">
      <img :src="banner.img" class="img-fluid" alt="Banner">
    </div>

    <div class="container d-flex justify-content-center">
      <div class="row align-items-start">
        <div 
          class="col d-flex justify-content-center" 
          v-for="(item, index) in cardImg" 
          :key="index">
          <a class="nav-link" href="#">
            <div class="cards">
              <div>
                <!-- Sección de títulos de la tarjeta -->
                <div class="card-titles">
                  <div class="card-headers">
                    <div class="card-mains">
                      <!-- Imagen dinámica obtenida de 'item.cardImg' -->
                      <img :src="item.cardImg" alt="Imagen de la tarjeta">
                    </div>
                  </div>
                </div>
                <!-- Texto dinámico asociado a la tarjeta -->
                <p>{{ item.Text }}</p>
              </div>
            </div>
          </a>
        </div>
      </div>
    </div>

    <!-- Botones -->
    <div class="boton d-flex justify-content-center">
      <button type="button" class="btn btn-1">Oficina Virtual</button>
      <button type="button" class="btn btn-2">Servicios</button>
    </div>
  </section>
  <!-- Fin de las tarjetas -->
</template>

<style>
/* Agrega tus estilos aquí */
</style>
