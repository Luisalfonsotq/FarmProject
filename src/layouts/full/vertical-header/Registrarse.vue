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
            text="Registrarse"
            v-bind="activatorProps"
          ></v-btn>
        </template>
  
        <v-card
          prepend-icon="mdi-account"
          title="Registrarse"
        max-height="900"

        >
          <v-card-text>
            <v-row>
               <v-col
                cols="12"
                md="4"
                sm="6"
              >
                <v-text-field
                  label="Email*"
                  required
                ></v-text-field>
              </v-col>
            </v-row>
            <v-row>
              <v-col
                cols="12"
                md="4"
                sm="6"
              >
                <v-text-field
                  label="Password*"
                  type="password"
                  required
                ></v-text-field>
              </v-col>
            </v-row>
            <v-row>
              <v-col
                cols="12"
                md="4"
                sm="6"
              >
                <v-text-field
                  label="Confirm Password*"
                  type="password"
                  required
                ></v-text-field>
              </v-col>
            </v-row>
            <small class="text-caption text-medium-emphasis">*indicates required field</small>
            <v-divider></v-divider>
        
            <v-row dense>
              <v-btn>hola2</v-btn>
            </v-row>
            <v-row>
              <v-btn>hola</v-btn>
            </v-row>
  
          </v-card-text>
          <v-divider></v-divider>
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
  import { shallowRef } from 'vue'

  const dialog = shallowRef(false)
</script>

<style>
.boton{
  background-color: white;
  color:black;
  
}
</style>