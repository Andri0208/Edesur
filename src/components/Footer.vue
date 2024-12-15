<script setup>

const img = {
    img1: 'public/logo.png.png',
}

</script>

<template>
<div class="container footer ">
  <div class="row align-items-start">
    <div class="col-xl-2 col-md-12 img">
        <img :src="img.img1" class="img-fluid" alt="imagen de edesur dominicana">
    </div>
    <div class="col">
        <div class="row">
            <div class="col-xl-3">
      <ul>
        <h5>CONÓCENOS</h5>
      </ul>
      <ul>
        <a class="nav-link" href="#">
            <p>Edesur Dominicana S.A</p>
            </a>
      </ul>
      </div>
      <div class="col-xl-3">
        <ul>
            <h5>CONTÁCTANOS</h5>
        </ul>
        <ul>
            <li>Tel: (809) 683-9292</li>
        </ul>
        <ul>
            <li>Fax: (809)-683-9393</li>
        </ul>
        <ul>
            <li>info@edesur.com.do</li>
        </ul>
      </div>
      <div class="col-xl-3">
        <ul>
            <h5>BÚSCANOS</h5>
        </ul>
        <ul>
            <p>Av. Tiradentes #47 Esq. Carlos Sánchez y
Sánchez, Torre Serrano, Ensanche Naco, Distrito
Nacional, República Dom.</p>
            </ul>

      </div>
      <div class="col-xl-3">
        <ul>
            <h5>INFÓRMATE</h5>
        </ul>
        <ul>
            <a class="nav-link" href="#">
            <p>Términos de Uso</p>
            </a>
        </ul>
        <ul>
            <a class="nav-link" href="#">
            <p>Políticas de Privacidad</p>
            </a>
        </ul>
        <ul>
            <a class="nav-link" href="#">
            <p>Preguntas Frecuentes</p>
            </a>
        </ul>
      </div>
      </div>
    </div>

  </div>
  
</div>
<footer class="">
    <div class="container d-flex justify-content-between align-items-center contenedor">
    <div>
    <p>© 2023 Todos los Derechos Reservados. Desarrollado por <span>Edesur Dominicana S.A</span></p>
    </div>
    <div class="d-flex align-items-center ">
        <p>SIGUENOS</p>
        <a href="#">
        <i class="fa-brands fa-facebook"></i>
        </a>
        <a href="#">
            <i class="fa-brands fa-twitter"></i>
        </a>
        <a href="#">
            <i class="fa-brands fa-instagram"></i> 
        </a>
        <a href="#">
            <i class="fa-brands fa-youtube"></i>
        </a>
    </div>
    </div>
  </footer>
</template>
<style>


</style>