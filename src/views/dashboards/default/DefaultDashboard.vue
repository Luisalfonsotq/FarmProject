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
    background:  $white;
    height: 500px;
    align-items: center;
  }

  @keyframes gradient{
    0%{
      background-position: 0% 50%;
    }
    50%{
      background-position: 100% 50%;
    }
    100%{
      background-position: 0% 50%;
    }
  }

  .fila{
    height: 500px;
    background: linear-gradient(-45deg,#D1E3B1, #25632d);
    background-size: 400% 400%;
     animation: gradient 15s ease infinite;
  }
 
  .card{
    display: grid;
    justify-content: center;
    align-content: center;
  }

</style>
