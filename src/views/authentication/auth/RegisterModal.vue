<template>
    <div>
      <v-btn @click="dialog = true" rounded="xl" elevation="2" class="ms-4">Registrarse</v-btn>
  
      <v-dialog v-model="dialog" max-width="900px">
        <v-card>
          <!-- <v-card-title class="headline">Componente en Modal</v-card-title> -->
          <v-card-text>
            <RegisterPage />
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
    import{ref} from 'vue'
    import RegisterPage from './RegisterPage.vue';
    const dialog = ref(false)
</script>