<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="danger">
      
      <b-img src="../assets/destacados/Negro.png" alt="EJG" class="logo-previo"></b-img>

      <b-navbar-brand href="">El Jonaz Games</b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          
            <b-nav-item href to="/Inicio">Inicio</b-nav-item>
            
          <b-nav-item-dropdown text="Categorias I" right>
            <b-dropdown-item href to="/JuegosAndroid">Juegos Android</b-dropdown-item>
            <b-dropdown-item href="#">2D</b-dropdown-item>
            <b-dropdown-item href="">32 Bits</b-dropdown-item>
            <b-dropdown-item href="#">3DS Rooms</b-dropdown-item>
            <b-dropdown-item href="#">Acción</b-dropdown-item>
            <b-dropdown-item href="#">Anime</b-dropdown-item>
            <b-dropdown-item href="#">Carreras</b-dropdown-item>
            <b-dropdown-item href="#">Construcción</b-dropdown-item>
            <b-dropdown-item href="#">Deportes</b-dropdown-item>
            <b-dropdown-item href="#">Estrategia</b-dropdown-item>
            <b-dropdown-item href="#">Shooter</b-dropdown-item>
            <b-dropdown-item href="#">Guerra</b-dropdown-item>
            <b-dropdown-item href to="/ListaProyectos">Lucha</b-dropdown-item>
          </b-nav-item-dropdown>

          <b-nav-item-dropdown text="Categorias II" right>
            <b-dropdown-item href="#">Multiplayer Online</b-dropdown-item>
            <b-dropdown-item href="#">Mundo Abierto</b-dropdown-item>
            <b-dropdown-item href="#">Pantalla Dividida</b-dropdown-item>
            <b-dropdown-item href="#">Pixelados</b-dropdown-item>
            <b-dropdown-item href to="/PS2">PS2 Rooms</b-dropdown-item>
            <b-dropdown-item href="#">PSP Rooms</b-dropdown-item>
            <b-dropdown-item href="#">Rol</b-dropdown-item>
            <b-dropdown-item href="#">Simulación</b-dropdown-item>
            <b-dropdown-item href="#">Supervivencia</b-dropdown-item>
            <b-dropdown-item href="#">Terror</b-dropdown-item>
            <b-dropdown-item href="#">VR</b-dropdown-item>
            <b-dropdown-item href="#">Wii Rooms</b-dropdown-item>
            <b-dropdown-item href="#">Zombies</b-dropdown-item>
          </b-nav-item-dropdown>

          <b-nav-item href to="#">Requisitos</b-nav-item>
          
          <b-nav-item-dropdown text="Programas para PC" right>
            <b-dropdown-item href="#">Emuladores</b-dropdown-item>
            <b-dropdown-item href="#">Sowfware</b-dropdown-item>
          </b-nav-item-dropdown>

          <b-nav-item-dropdown text="Ayuda" right>
            <b-dropdown-item href="#">¿Cómo Descargar?</b-dropdown-item>
            <b-dropdown-item href="#">¿Cómo Instalar?</b-dropdown-item>
            <b-dropdown-item href="#">Programas necesarios para jugar en PC</b-dropdown-item>
          </b-nav-item-dropdown>
          
        </b-navbar-nav>
        
        

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          
          <b-nav-item-dropdown text="Idioma" right>
            <b-dropdown-item href="#">EN</b-dropdown-item>
            <b-dropdown-item href="#">CAT</b-dropdown-item>
          </b-nav-item-dropdown>
          

          <b-nav-item-dropdown right>
            <!-- Using 'button-content' slot -->
            <template #button-content>
              <em>Usuario</em>
            </template>
            <b-dropdown-item href="#">Perfil</b-dropdown-item>
            <b-dropdown-item href="#">Cerrar Cuenta</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  // Puedes agregar lógica adicional aquí si es necesario
};
</script>

<style scoped>
/* Estilo para la nueva imagen previa */
.logo-previo {
  width: 30px;
  height: 30px;
  margin-right: 5px;
}

/* Estilo para reducir altura de la barra de navegación */
.b-navbar {
  height: 40px;
}

/* Estilo para reducir altura de los elementos de la barra de navegación */
.b-navbar-nav .nav-item {
  line-height: 10px;
  margin-bottom: 5px;
  font-size: 2px; /* Tamaño de fuente ajustado */
}
</style>