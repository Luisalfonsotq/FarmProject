<script setup lang="ts">
import { shallowRef } from 'vue';

const footerLink = shallowRef([
  {
    title: 'Home',
    url: 'https://berrydashboard.io/vue/free'
  },
  {
    title: 'Documentation',
    url: 'https://codedthemes.gitbook.io/berry-vuetify/'
  },
  {
    title: 'Support',
    url: 'https://codedthemes.support-hub.io/'
  }
]);

const currentDate = new Date();
const year = currentDate.getFullYear()

</script>
<template>
  <v-footer class="px-0 footer mt-2">
    <v-row justify="center" align="center" no-gutters>

      <v-col cols="12" sm="4">
        <p class="text-body-1 mb-0 text-sm-left text-center">
          HERDIX ♥ edited by Team:
          <a href="https://github.com/Luisalfonsotq/FarmProject.git" class="text-darkText text-decoration-none" target="_blank">El cuarteto</a>
        </p>
      </v-col>

      <v-col cols="12" sm="4">
        <p>Todos los derechos reservados {{ year }}</p>
      </v-col>
      <v-col class="text-sm-right text-center" cols="12" sm="4">
        <a
          v-for="(item, i) in footerLink"
          :key="i"
          class="mx-2 text-body-1 text-darkText text-decoration-none"
          target="_blank"
          :href="item.url"
        >
          {{ item.title }}
        </a>
      </v-col>
    </v-row>
  </v-footer>
</template>

<style lang="scss">
.v-footer {
  position: unset;
}
footer {
  a {
    &:hover {
      color: rgb(var(--v-theme-primary)) !important;
    }
  }
}
</style>
