<script setup lang="ts">
// import Logo from '@/layouts/full/logo/LogoDark.vue';
import AuthLogin from '../authForms/AuthLogin.vue';
</script>

<template>
  <v-row class="h-screen" no-gutters>
    <!---Left Part-->
    <v-col cols="12" class="d-flex align-center">
      <v-container >
        <div class="pa-3 pa-sm-10">
          <v-row justify="center" >
            <v-col cols="12" lg="10" xl="6" md="7">
              <v-card elevation="0" class="loginBox contenedor" rounded="xl">
                <v-card variant="outlined">
                  <v-card-text class="pa-9">
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
                    <AuthLogin />
                    <!---Left Part Form-->
                  </v-card-text>
                </v-card>
              </v-card>
            </v-col>
          </v-row>
        </div>
      </v-container>
    </v-col>
    <!---Left Part-->
  </v-row>
</template>
<style lang="scss">
.loginBox {
  max-width: 475px;
  margin: 0 auto;
}
.titulo2{
  color: $verdeHerdixOscuro;
}
.contenedor{
  background-color: $verdeHerdixClaro;
  // border-radius: 100px;
}
</style>
