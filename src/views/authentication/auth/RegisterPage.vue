<script setup lang="ts">
import Logo from '@/layouts/full/logo/LogoDark.vue';
import AuthRegister from '../authForms/AuthRegister.vue';
</script>

<template>
  <v-row class="h-screen" no-gutters>
    <!---Left Part-->
    <v-col cols="12" class="d-flex align-center bg-lightprimary">
      <v-container>
        <div class="pa-1 pa-sm-12">
          <v-row justify="center">
            <v-col cols="12" lg="10" xl="6" md="7">
              <v-card elevation="0" class="loginBox">
                <v-card variant="outlined">
                  <v-card-text class="pa-9">
                    <!---Left Part Logo -->
                    <v-row>
                      <v-col cols="12" class="text-center">
                        <Logo />
                        <h2 class="text-secondary text-h2 mt-8">Bienvenido a Herdix </h2>
                        <h4 class="text-disabled text-h4 mt-3"> Lleva tu finca al proximo nivel</h4>
                      </v-col>
                    </v-row>
                    <!---Left Part Logo -->

                    <!---Left Part Form-->
                    <AuthRegister />
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
  max-width: 500px;
  margin: 0 auto;
}
</style>
