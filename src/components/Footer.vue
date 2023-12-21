<template>
  <footer>
    <div class="footer-content">
      <div class="left-section">
        <img src="@/assets/destacados/EJGnegro (1).svg" alt="El Jonaz Games" class="first-image" />
        <img src="@/assets/destacados/Logo.png" alt="El Jonaz Games" class="second-image" />
      </div>
      <div class="right-section">
        
        <!-- Primera sección -->
        <div class="footer-section">
          <h4>Información</h4>
          <div class="row-section">
            <h5>Rambla Ferrán 33 3r 3a</h5>
            <h5>666 66 66 66</h5>
            <h5>info@eljonazgames.com</h5>
          </div>
        </div>

        <!-- Segunda sección -->
        <div class="footer-section">
          <h4>Sobre nosotros</h4>
          <div class="row-section">
            <h5>¿Cómo trabajamos?</h5>
            <h5>Especialidades</h5>
          </div>
        </div>

        <!-- Tercera sección -->
        <div class="footer-section">
          <h4>Ayuda</h4>
          <div class="row-section">
            <h5>Privacidad</h5>
            <h5>Cookies</h5>
          </div>
        </div>
      </div>
      
    </div>
  </footer>
</template>

<script>

</script>

<style scoped>
footer {
  background-color: #dc3545; /* Cambiado a rojo */
  color: #000000; /* Color del texto en el footer */
  padding: 20px 0; /* Ajusta el relleno según tus preferencias */
  text-align: center;
}

.footer-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px; /* Ancho máximo del contenido del footer */
  margin: 0 auto; /* Centra el contenido horizontalmente */
}

.first-image {
  width: 80px; /* Ajusta el ancho de la primera imagen según tus preferencias */
  height: 100px; /* Ajusta la altura de la primera imagen según tus preferencias */
  margin-right: 10px; /* Ajusta el margen entre las imágenes según tus preferencias */
  margin-left: -50px;
}

.second-image {
  width: 70px; /* Ajusta el ancho de la segunda imagen según tus preferencias */
  height: 70px; /* Ajusta la altura de la segunda imagen según tus preferencias */
  margin-left: -30px;
}

/* Estilos de la sección de la fila */
.row-section {
  display: flex;
  flex-direction: column; /* Cambia la dirección del flexbox a columna */
  align-items: center; /* Centra los enlaces horizontalmente */
}

/* Ajustes adicionales según tus preferencias */
.row-section h5 {
  font-size: 15px;
  margin-bottom: 5px; /* Espacio entre los enlaces */
  text-decoration: none; /* Quita el subrayado del enlace si es necesario */
}

.footer-section {
  margin-top: 0px;
  text-align: center; /* Centra el texto dentro de cada sección */
  width: 33%; /* Ajusta el ancho de cada sección para que ocupen el espacio deseado */
}

/* Añade la siguiente regla para que las secciones estén una al lado de la otra */
.right-section {
  display: flex;
  width: 80%;
  justify-content: center;
}

/* Estilos para pantallas pequeñas */
@media screen and (max-width: 768px) {
  .footer-section {
    width: 100%; /* Ocupa el ancho completo en pantallas pequeñas */
    margin-bottom: 20px; /* Espacio entre las secciones en pantallas pequeñas */
  }

  .right-section {
    width: 100%;
  }

  .left-section {
    text-align: center; /* Centra las imágenes en pantallas pequeñas */
  }
}
</style>
