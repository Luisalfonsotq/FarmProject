<template>
    <div>
      <v-btn @click="dialog = true" rounded="xl" elevation="2" class="ms-4 boton">Iniciar Sesión</v-btn>
  
      <v-dialog v-model="dialog" max-width="900px">
        <v-card class="modal-card">
          <v-card-text>
            <LoginPage/>
          </v-card-text>
          <v-card-actions>
            <v-spacer />
            <v-btn color="primary" @click="dialog = false">Cerrar</v-btn>
          </v-card-actions>
        </v-card>
      </v-dialog>
    </div>
  </template>

  <script setup>
  import { ref } from 'vue'
import LoginPage from '../LoginPage.vue';
  const dialog = ref(false)
</script>

<style>
.boton{
  background-color: #d1e3b1;
}

  .modal-card {
    background-color: white !important;
}


</style>