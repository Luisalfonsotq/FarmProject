<script setup lang="ts">
  import { RouterView } from 'vue-router';
  import VerticalSidebarVue from './vertical-sidebar/VerticalSidebar.vue';
  import VerticalHeaderVue from './vertical-header/VerticalHeader.vue';
  import CustomizerPanel from './customizer/CustomizerPanel.vue';
  import FooterPanel from './footer/FooterPanel.vue';
  import { useCustomizerStore } from '../../stores/customizer';
  const customizer = useCustomizerStore();
</script>

<template>
  <v-locale-provider>
    <v-app
      theme="PurpleTheme"
      :class="[customizer.fontTheme, customizer.mini_sidebar ? 'mini-sidebar' : '', customizer.inputBg ? 'inputWithbg' : '']"
    >
      <CustomizerPanel />
      <!-- Nav bar -->
      <VerticalHeaderVue />
      <!-- Side bar -->
      <VerticalSidebarVue />

      <v-main>
        <v-container fluid class="page-wrapper">
          <div>
            <!-- Rutas -->
            <RouterView />
            <v-btn
              class="customizer-btn"
              size="large"
              icon
              variant="flat"
              color="secondary"
              @click.stop="customizer.SET_CUSTOMIZER_DRAWER(!customizer.Customizer_drawer)"
            >
              <SettingsIcon class="icon" />
            </v-btn>
          </div>
        </v-container>
        <!-- Footer -->
        <v-container fluid class="pt-0">
          <div>
            <FooterPanel />
          </div>
        </v-container>

      </v-main>
    </v-app>
  </v-locale-provider>
</template>

<style lang="scss" scoped>
.page-wrapper{
  background-color: $white;
}

</style>
