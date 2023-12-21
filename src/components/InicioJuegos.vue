<template>
  
    <div class="main-page-container">
    
      <!-- Container 1: Más jugados esta semana -->
      <div class="container container1">
        <div class="content">
          <div class="featured-games">
            <h2>🎮 ¡MÁS JUGADOS ESTA SEMANA! 🎮</h2>
            <div class="game-row">
              <!-- Primera Fila -->
              <div class="game">
                <img src="../assets/destacados/gta6.jpg" alt="GTA6" />
                <p>Gta VI</p>
              </div>
              <div class="game">
                <img src="../assets/destacados/phasmo.jpeg" alt="PHASMOPHOBIA" />
                <p>Phasmophobia</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    
      <!-- Container 2: Menos jugados -->
      <div class="container container2">
        <div class="content">
          <h2>🎮 ¡MÁS BUSCADOS! 🎮</h2>
          <!-- Nueva Columna -->
          <div class="game-row1">
            <!-- Primera Fila -->
            <div class="game2">
              <img src="../assets/destacados/Among.jpg" alt="Among Us" />
              <p>Among Us</p>
            </div>
            <div class="game2">
              <img src="../assets/destacados/CSGO.jpg" alt="CSGO" />
              <p>CSGO</p>
            </div>
            <div class="game2">
              <img src="../assets/destacados/FIFA24.jpg" alt="FIFA 24" />
              <p>FIFA 24</p>
            </div>
            <div class="game2">
              <img src="../assets/destacados/Minecraft.jpg" alt="Minecraft" />
              <p>Minecraft</p>
            </div>
            <!-- Segunda Fila -->
            <div class="game2">
              <img src="../assets/destacados/Plants.jpg" alt="Plants Vs Zombies" />
              <p>Plants Vs Zombies</p>
            </div>
            <div class="game2">
              <img src="../assets/destacados/Raft.jpg" alt="Raft" />
              <p>Raft</p>
            </div>
            <div class="game2">
              <img src="../assets/destacados/Stumble.jpg" alt="Stumble Guys" />
              <p>Stumble Guys</p>
            </div>
            <div class="game2">
              <img src="../assets/destacados/Habbo.jpg" alt="Habbo Hotel" />
              <p>Habbo Hotel</p>
            </div>

            <!-- Tercera Fila -->
            <div class="game2">
              <img src="../assets/destacados/Pokemon.jpg" alt="Pokemon United" />
              <p>Pokemon United</p>
            </div>
            <div class="game2">
              <img src="../assets/destacados/Wicher.jpg" alt="The Witcher" />
              <p>The Witcher</p>
            </div>
            <div class="game2">
              <img src="../assets/destacados/War.jpg" alt="War Of Warships" />
              <p>War Of Warships</p>
            </div>
            <div class="game2">
              <img src="../assets/destacados/Lord.png" alt="Lord Of The Ring" />
              <p>Lord Of The Ring</p>
            </div>
          </div>
        </div>
      </div>

      <div class="horizontal-line"></div>

      <!--Carrusel-->
      <div>
        <h1>📷¡CAPTURAS JUEGOS MÁS JUGADOS!📷</h1>

        <b-carousel
            id="carousel-1"
            v-model="slide"
            :interval="4000"
            controls
            indicators
            background="#ababab"
            img-width="1280"
            img-height="720"
            style="text-shadow: 1px 1px 2px #333;"
            @sliding-start="onSlideStart"
            @sliding-end="onSlideEnd"
            >

            <!-- Slides with custom text -->
            <b-carousel-slide img-src="@/assets/Carrusel/GTA6.jpg"></b-carousel-slide>   

            <b-carousel-slide img-src="@/assets/Carrusel/Phasmo1.jpg"></b-carousel-slide>    
          
            <b-carousel-slide img-src="@/assets/Carrusel/6GTA.jpg"></b-carousel-slide>

            <b-carousel-slide img-src="@/assets/Carrusel/Phasmo2.jpg"></b-carousel-slide>
        </b-carousel>
      </div>

      <div class="horizontal-line"></div>

       <h2 class="Valoración">Déjanos tu valoración y comenta</h2>

        <div>
            <b-form-rating v-model="value"></b-form-rating>
        </div>

      <!--Prueba-->    
      <div class="custom-container">
        <img src="@/assets/Chat/Comentario.jpg" alt="Comentarios" style="width: 100%; height: 100%;" />
      </div>

  </div>
</template>

<script>
  export default {
    data() {
      return {
        value: null
      }
    }
  }
</script>

<style lang="scss">


/*Texto Valora*/
.Valoración{
  margin-top: 1rem;
  color: red;
  font-size: 20px; /* Tamaño de fuente ajustado */
  margin-bottom: 25px;
}

/*Carrusel*/
#carousel-1 {
    margin-top: 20px; /* Ajusta el margen superior según tus necesidades */
    margin-bottom: 20px; /* Ajusta el margen inferior según tus necesidades */
    max-width: 800px; /* Ajusta el tamaño máximo del carrusel según tus necesidades */
    margin-left: auto; /* Centra el carrusel horizontalmente */
    margin-right: auto; /* Centra el carrusel horizontalmente */
  }

/*Letra Texto Carrusel*/
  h1 {
    color: red; /* Cambia el color del texto a rojo */
    text-align: center; /* Centra el texto horizontalmente */
    margin-top: 10px; /* Ajusta el margen superior según tus necesidades */
  }
  
/*Linea Separadora Blanca*/
.horizontal-line {
  border-top: 1px solid #ffffff; /* Estilo de la línea: 1 píxel de ancho y blanco */
  margin-top: 10px ; /*Espacio superior e inferior de la línea */
}

/*Contenedor principal */
.main-page-container {
  background-color: #151414; /* Fondo negro */
  max-width: 80%; /* Ocupa el 80% de la página */
  margin: 0 auto; /* Centrado horizontalmente */
  padding: 20px; /* Ajusta según sea necesario */
}

.container1 {
  max-width: 1200px; /* Puedes ajustar el ancho máximo según tus necesidades */
  margin: 0 auto;
  display: center;
  justify-content: space-between;
}

.container2 {
  max-width: 1400px; /* Puedes ajustar el ancho máximo según tus necesidades */
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
}

.container2 h2{
  text-align: center;
}

.container1,
.container2 {
  width: 100%; /* Ajusta el ancho según tus necesidades */
}

.featured-games {
  text-align: center;
}

.section-title {
  margin-bottom: 20px;
}

.game-row1 {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap; /* Para que las imágenes se envuelvan cuando no haya suficiente espacio */
}

.game-row {
  display: flex;
  justify-content: center;
  flex-wrap: wrap; /* Para que las imágenes se envuelvan cuando no haya suficiente espacio */
}

.game,
.game2 {
  margin: 5px;
  text-align: center; /* Centra el texto dentro de cada juego */
}

/* Tamaño de las fotos de destacados */
.game img {
  width: 300px;
  height: 200px;
  object-fit: cover;
}

.game2 img {
  width: 180px;
  height: 100px;
  object-fit: cover;
}


.game2 p {
  margin-top: 0.5rem;
  color: white;
  font-size: 12px; /* Tamaño de fuente ajustado */
}

.game p{
  margin-top: 0.6rem;
  color: white;
  font-size: 16px; /* Tamaño de fuente ajustado */
}

.content h2 {
  margin-top: 1rem;
  color: red;
  font-size: 20px; /* Tamaño de fuente ajustado */
}

.background {
  width: 100%;
  height: 820px;
  margin-top: -20px;
  background-color: rgb(43, 43, 43, 0.95); /* Color gris */
  position: absolute;
  top: 0;
  left: 0;
  z-index: -2; /* Colocar el fondo debajo de todo */
}

.publi{

  height: 300px;
  width: 220px;

}

@media screen and (max-width: 768px) {


  .container2 {
    flex-direction: column; /* Cambia la dirección de la columna en pantallas pequeñas */
  }

}


@media screen and (max-width: 1241px) {
   .background {
    height: 955px;
    margin-top: 100px;
  }
  .publi{

    height: 200px;
    width: 146px;

  }  

}

@media screen and (max-width: 920px) {
   .background {
    height: 1270px;
  }
    
}

  @media screen and (max-width: 920px) {
   .background {
    height: 1270px;
  }
  }

  @media screen and (max-width: 812px) {
   .background {
    height: 1530px;
  }
  }

</style>