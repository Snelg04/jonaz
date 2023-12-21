<template>
  <div id="app">
    <nav>
      <Navbar></Navbar>
      
    </nav>
    <router-view/>
     <div id="fullscreen-container">
      <!-- Imagen dentro del contenedor -->
      <img src="@/assets/destacados/sss.jpeg" alt="FONDO" />
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'Cositas',
  components: {
    Navbar,
    Footer
  
  }
}
</script>

<style>
body {
  margin: 0; /* Asegura que no haya márgenes en el cuerpo */
}

#fullscreen-container {
  position: fixed; /* Fija el contenedor a la ventana del navegador */
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: -1; /* Coloca el contenedor detrás del contenido principal */
}

#fullscreen-container img {
  width: 100%; /* Ajusta el ancho de la imagen al 100% del contenedor */
  height: 100%; /* Ajusta la altura de la imagen al 100% del contenedor */
  object-fit: cover; /* Ajusta la imagen para cubrir completamente el contenedor */
}

nav {
  position: relative; /* Establece posición relativa para el nav */
  z-index: 1; /* Asegura que el nav esté por encima de la imagen de fondo */
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
