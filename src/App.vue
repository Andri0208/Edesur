<script setup>
import AppMovil from './components/AppMovil.vue';
import Certificaciones from './components/Certificaciones.vue';
import Contactanos from './components/Contactanos.vue';
import Footer from './components/footer.vue';
import Headers from './components/Headers.vue';
import InformacionAlCliente from './components/informacionAlCliente.vue';
import Licitacion from './components/licitacion.vue';
import Mains from './components/mains.vue';
import Noticias from './components/Noticias.vue';
</script>

<template>
  <div class="edesur">
<Headers/>
<Mains/>
<InformacionAlCliente/>
<AppMovil/>
<Noticias/>
<Licitacion/>
<Certificaciones/>
<Contactanos/>
<Footer/>
</div>

</template>

<style>

</style>