<script setup lang="ts">
import Carrusel from './components/Carrusel.vue';
import Tarjeta from './components/Tarjeta.vue';
import Nosotros from './components/Nosotros.vue';

</script>

<template>
  <v-row justify="center" class="fila">
    
    <v-col cols="12" md="5">
      <Carrusel />
    </v-col>

    <v-col cols="6" md="5" class="card">
      <Tarjeta />
    </v-col>
 
  </v-row>
  <br>
  <v-row class="fila1 text-white justify-center" cols="12" md="5" >
    <div >
      <Nosotros/>
    </div>
  </v-row>

 
</template>

<style scoped lang="scss">
  .fila{
    background:  $verdeHerdixClaro;
    height: 500px;
    align-items: center;
  }
 
  .card{
    display: grid;
    justify-content: center;
    align-content: center;
  }

</style>
