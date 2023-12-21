<!--Hace referencia a todo aquello que se puede observar cuando pulsas o estas en el apartado Inicio-->
<template>
  <div class="Inicio">
   <InicioJuegos></InicioJuegos>
  </div>
</template>

<script>
import InicioJuegos from '../components/InicioJuegos.vue';


export default {
  name: 'Cositas',
  components: {
    InicioJuegos,
  }
}

</script>
