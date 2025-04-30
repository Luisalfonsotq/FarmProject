<template>
    <div class="text-center">
      <v-dialog
        v-model="dialog"
        max-width="600"
      >
        <template v-slot:activator="{ props: activatorProps }">
          <v-btn
            class="ms-4"
            rounded="xl" 
            elevation="2"
            variant="flat"
            text="Registrer"
            v-bind="activatorProps"
          ></v-btn>
        </template>
  
        <v-card
          prepend-icon="mdi-account"
          title="Registrarse"
        max-height="auto"

        >
        <div class="conte">
       <!--   <RegisterPage/> -->
          <AuthLogin/>
        </div>

          <v-card-actions>
            <v-spacer></v-spacer>

            <v-btn
              text="Close"
              variant="plain"
              @click="dialog = false"
            ></v-btn>
  
            <v-btn
              color="primary"
              text="Save"
              variant="tonal"
              @click="dialog = false"
            ></v-btn>
          </v-card-actions>
        </v-card>
      </v-dialog>
    </div>
  </template>
  <script setup>
 // import RegisterPage from '@/views/authentication/auth/RegisterPage.vue';
import AuthLogin from '@/views/authentication/authForms/AuthLogin.vue';
import { shallowRef } from 'vue'

  const dialog = shallowRef(false)
</script>

<style scoped lang="scss">
// .boton{
//   background-color: $verdeHerdixOscuro;
//   // color:black;
  
// }

.conte{
  background-color: $verdeHerdixOscuro;
}
</style>