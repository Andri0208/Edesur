<script setup>
const img = {
    logo: 'public/logo.png.png',
    grid: 'src/assets/grid-menu-icon.svg.png',
    favicon: 'public/favicon.png.png' 
}
</script>

<template>
  <header class="base">
    <div class="d-flex justify-content-between header-container container">
      <!-- Logo y nombre -->
      <div class="d-flex header-logo">
        <img :src="img.logo" class="img-fluid logo" alt="Logo de Edesur Dominicana">
        <p class="fs-4 titulo-header">Edesur Dominicana, S.A.</p>
      </div>

      <!-- Barra de búsqueda y botón grid -->
      <div class="header-search d-flex align-items-center">
        <form class="d-flex" role="search">
          <input id="search-1" class="form-control" type="search" placeholder="¿Qué quieres buscar?" aria-label="Search">
          <button class="btn btn-danger btn-search" type="submit">
            <i class="fa-solid fa-magnifying-glass"></i>
          </button>
        </form>
        <button class="btn btn-grid">
          <img :src="img.grid" alt="Icono del menú en cuadrícula">
        </button>
      </div>
    </div>

    <!-- Navbar -->
     <div class=" color-navbar">
      <nav class="navbar navbar-expand-lg bg-body-tertiary container">
      <div class="container-fluid navegacion">
        <a class="navbar-brand na" href="#">
          <img id="favicon" :src="img.favicon" alt="Img del navbar" /> Inicio
        </a>

        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <!-- Botón desplegable: Sobre Nosotros -->
            <li class="nav-item dropdown">
              <a
                class="nav-link dropdown-toggle"
                href="#"
                role="button"
                data-bs-toggle="dropdown"
                aria-expanded="false"
              >
                Sobre Nosotros
              </a>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">¿Quiénes somos?</a></li>
                <li><a class="dropdown-item" href="#">Historia</a></li>
                <li><a class="dropdown-item" href="#">Organigrama</a></li>
                <li>
                  <a class="dropdown-item" href="#">Carta de compromiso</a>
                </li>
                <li>
                  <a class="dropdown-item" href="#"
                    >Despacho del Administrador</a
                  >
                </li>
                <li><a class="dropdown-item" href="#">Marco legal</a></li>
                <li>
                  <a class="dropdown-item" href="#">Política integrada</a>
                </li>
              </ul>
            </li>

            <!-- Otros enlaces -->
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#"
                >Servicios</a
              >
            </li>
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#"
                >Transparencia</a
              >
            </li>

            <!-- Botón desplegable: Proyecto -->
            <li class="nav-item dropdown">
              <a
                class="nav-link dropdown-toggle"
                href="#"
                role="button"
                data-bs-toggle="dropdown"
                aria-expanded="false"
              >
                Proyecto
              </a>
              <ul class="dropdown-menu">
                <li>
                  <a class="dropdown-item" href="#"
                    >Punto de informacion Ciudadana</a
                  >
                </li>
                <li>
                  <a class="dropdown-item" href="#">Responsabilidad Social</a>
                </li>
                <li><a class="dropdown-item" href="#">Gestion Social</a></li>
              </ul>
            </li>

            <!-- Otros enlaces -->
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#"
                >Noticias</a
              >
            </li>

            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#">Blog</a>
            </li>
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#">Foro</a>
            </li>
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#"
                >Oficina Virtual</a
              >
            </li>
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#"
                >Contacto</a
              >
            </li>
          </ul>
        </div>
      </div>
    </nav>
</div>

  </header>
</template>



<style>


</style>