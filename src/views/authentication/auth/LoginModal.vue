<template>
    <div>
      <v-btn @click="dialog = true" rounded="xl" elevation="2" class="ms-4 boton">Iniciar Sesión</v-btn>
  
      <v-dialog v-model="dialog" max-width="400px">
        <v-card-text class="tarjeta" >
                    <!---Left Part Logo -->
                    <v-row>
                      <v-col cols="12" class="text-center">
                        <img 
                        src="/public/HERDIX.svg"
                        width="150"
                        height="150"/>
                        <!-- <Logo /> -->
                        <h2 class=" text-h2 mt-4 titulo2">Lleva tu finca al proximo nivel</h2>
                        <h4 class="text-disabled text-h4 mt-3">Ingrese su usuario</h4>
                      </v-col>
                    </v-row>
                    <!---Left Part Logo -->

                    <!---Left Part Form-->
                    <LoginPage />
                    <!---Left Part Form-->
                  </v-card-text>
      </v-dialog>
    </div>
  </template>

  <script setup>
  import { ref } from 'vue'
import LoginPage from '@/views/authentication/authForms/AuthLogin.vue';
  const dialog = ref(false)
</script>

<style>
.tarjeta{
  background-color: #d1e3b1;
  border-radius: 40px;
}
.boton{
  background-color: #d1e3b1;
}

  .modal-card {
    background-color: white !important;
}


</style>