<script setup lang="ts">
// imported components
// import TotalEarning from './components/TotalEarning.vue';
// import TotalOrder from './components/TotalOrder.vue';
// import TotalIncome from './components/TotalIncome.vue';
// import TotalGrowth from './components/TotalGrowth.vue';
// import PopularStocks from './components/PopularStocks.vue';
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
 
   
    
  
    <!-- -------------------------------------------------------------------- -->
    <!-- Total Earning -->
    <!-- -------------------------------------------------------------------- -->
    <!-- <v-col cols="12" md="4">
      <TotalEarning /> 
    </v-col> -->
    <!-- -------------------------------------------------------------------- -->
    <!-- Total Order -->
    <!-- -------------------------------------------------------------------- -->
    <!-- <v-col cols="12" md="4">
      <TotalOrder />
    </v-col> -->
    <!-- -------------------------------------------------------------------- -->
    <!-- Total Income -->
    <!-- -------------------------------------------------------------------- -->
    <!-- <v-col cols="12" md="4">
      <TotalIncome />
    </v-col> -->

    <!-- -------------------------------------------------------------------- -->
    <!-- Total Growth -->
    <!-- -------------------------------------------------------------------- -->
    <!-- <v-col cols="12" lg="8">
      <TotalGrowth />
    </v-col> -->

    <!-- -------------------------------------------------------------------- -->
    <!-- Popular Stocks -->
    <!-- -------------------------------------------------------------------- -->
    <!-- <v-col cols="12" lg="4">
      <PopularStocks />
    </v-col> -->
  </v-row>
  <br>
  <v-row class="fila1 text-white justify-center" cols="12" md="5" >
    <div >
      <Nosotros/>
    </div>
  </v-row>

 
</template>

<style scoped>
  .fila{
    background: #D1E3B1;
    height: 500px;
    align-items: center;
  }
 
  .card{
    display: grid;
    justify-content: center;
    align-content: center;
  }

</style>
