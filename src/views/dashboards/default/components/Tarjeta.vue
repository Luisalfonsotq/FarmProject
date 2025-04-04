<template>
  <div class="empanada">
    <div class="seccion">
      <img 
       :width="400"
      aspect-ratio="16/9" 
      class="logo" src="/public/HERDIX-LOGO-copia.svg">
    </div>
    <div class="seccion">

      <p class="text-center text-h2">¡Descubre la forma más fácil y eficiente de administrar tu finca con Herdix!</p>
    </div>

  </div>
  <!-- <v-card
      class="mx-auto text-white"
      color="#b88917"
      max-width="600"
      prepend-icon="mdi-twitter"
      title="¡Convierte tus ideas en acción!"
    >
      <template v-slot:prepend>
        <v-icon size="x-large"></v-icon>
      </template>

<v-card-text class="text-h4 py-2">
  "Diseña potreros únicos, programa eventos clave y recibe notificaciones personalizadas en tu finca digital. Simplifica
  la gestión y lleva tu negocio al siguiente nivel."
</v-card-text>

<v-card-actions>
  <v-list-item class="w-100">
    <template v-slot:prepend>
            <v-avatar
              color="grey-darken-3"
              image="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light"
            ></v-avatar>
          </template>

    <v-list-item-title>Evan You</v-list-item-title>

    <v-list-item-subtitle>Vue Creator</v-list-item-subtitle>

    <template v-slot:append>
            <div class="justify-self-end">
              <v-icon class="me-1" icon="mdi-heart"></v-icon>
              <span class="subheading me-2">256</span>
              <span class="me-1">·</span>
              <v-icon class="me-1" icon="mdi-share-variant"></v-icon>
              <span class="subheading">45</span>
            </div>
          </template>
  </v-list-item>
</v-card-actions>
</v-card> -->
</template>
<style scoped>
.empanada {
  height: auto;
  width: 350px;
  background: transparent;
  display: flex;
  flex-direction: column;
align-items: center;
}
.empanada *{
  width: 100%;
}
.empanada>div:first-child{

  width: 200px !important;
  height: auto;
}
.empanada>div:last-child>p{
  background: white;
  padding: 10px;
  height: 150px;
  border-bottom-left-radius: 180px;
  border-bottom-right-radius: 180px;
}
.logo{
  width: 100%;
  height: auto;
  
}

</style>