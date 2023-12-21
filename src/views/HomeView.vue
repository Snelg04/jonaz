<!--Hace referencia a todo aquello que se puede observar al abrir el documento-->
<template>
  <div class="center-container">
    <div class="center">
      <div id="ui">
        <div id="ui-right">
          <h1>Regístrate</h1>
          <div class="split-s"></div>
          <h2>PARA PODER JUGAR</h2>
          <br>
          <br>
          <br>
          <br>
          <div class="split-l"></div>
          <p>No tienes cuenta?</p>
          <a href="#">Registrate</a>
        </div>
        <form id="ui-left">
          <h3>Iniciar Sesión</h3>
          <div class="split-l"></div>
          <label for="name">
            <i class="material-icons"></i>
          </label>
          <br>
          <input id="name" placeholder="Usuario" ref="usuario">
          <div class="split-m"></div>
          <label for="pass1">
            <i class="material-icons"></i>
          </label>
          <br>
          <input id="pass1" placeholder="Contraseña" type="password" ref="contraseña">
          <div class="split-m"></div>
          <br>
          <!-- Utiliza la directiva @click para manejar el clic en el botón -->
          <input type="button" value="Iniciar Sesión" @click="iniciarSesion">
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    iniciarSesion() {
      // Obtén los valores de usuario y contraseña desde los campos de entrada
      const usuario = this.$refs.usuario.value;
      const contraseña = this.$refs.contraseña.value;

      // Verifica las condiciones (en este caso, usuario debe ser "Afra" y contraseña debe ser "Afra")
      if (usuario === "Afra" && contraseña === "Afra") {
        // Si las condiciones son verdaderas, navega a la página de inicio
        this.$router.push("/Inicio");
      } else {
        // De lo contrario, realiza alguna acción (por ejemplo, muestra un mensaje de error)
        alert("Usuario o contraseña incorrectos");
      }
    }
  }
};
</script>

<style scoped>
body {
  margin: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
}

.center-container {
  text-align: center;
  margin-top: 5%;
  margin-bottom: 100px;
}

#pen-title {
  font-size: 40px;
  font-weight: 300;
  text-transform: uppercase;
  letter-spacing: 1px;
  word-spacing: 6px;
}

#ui {
  display: flex;
  justify-content: center;
  align-items: center;
}

#ui-right,
#ui-left {
  padding: 40px;
}

/*Cuadro Izquierda*/
#ui-right {
  width: 300px;
  background: #151414;
  text-align: left;
  box-shadow: 0px 6px 10px 0px rgba(0, 0, 0, 0.14),
    0px 1px 18px 0px rgba(0, 0, 0, 0.12), 0px 3px 5px -1px rgba(0, 0, 0, 0.3);
  z-index: 90;
}

/*Todos los Textos Del Cuadro De La Izquierda*/
#ui-right h1,h2,p, a{
  margin-left: -20px;
}

/*Texto Regístrate Cuadro Izquierda*/
h1 {
  margin-top: -20px;
  font-size: 40px;
  color: rgb(255, 0, 0);
  text-transform: uppercase;
}

/*Texto Poder Jugar Cuadro Izquierda*/
h2 {
  font-size: 20px;
  color: rgb(255, 0, 0);
  text-transform: uppercase;
}

/*Color de No tienes Cuenta? y de Regristrarse*/
#ui-right p,
#ui-right a {
  color: rgb(255, 0, 0);
  margin-bottom: 2px;
  font-size: 17px;
  font-weight: 700;
}

/*Cuadro Derecha*/
#ui-left {
  width: 300px;
  background: #ff0000;
  box-shadow: 0px 16px 24px 2px rgba(0, 0, 0, 0.14),
    0px 6px 30px 5px rgba(0, 0, 0, 0.12), 0px 8px 10px -5px rgba(0, 0, 0, 0.3);
  z-index: 91;
}

/*Texto Iniciar Sesión Cuadro Derecha*/
#ui-left h3 {
  color: #151414;
  font-size: 20px;
  text-transform: capitalize;
}

/*Borde Del Usuario y Contraseña */
input {
  border: 1px solid #151414;
}

input:hover,
input:focus {
  border: 1px solid rgba(0, 0, 0, 0.54);
}

/*Color de dentro del botón de Iniciar Sesión*/
input[type="button"] {
  color: rgb(255, 0, 0);
  background: rgba(0, 0, 0, 0.87);
  border: 1px solid rgba(0, 0, 0, 0.87);
}

/*Color cuando pones el ratón encima de Iniciar Sesión*/
input[type="button"]:hover {
  color: rgba(0, 0, 0, 0.87);
  background: #ffffff;
  border: 1px solid #000000;
}
</style>
