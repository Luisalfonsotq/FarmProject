<template>
  <v-card class="mx-auto card-carousel rounded-md" elevation="" max-width="444">
    <v-carousel 
    :continuous="false" 
    :show-arrows="false" 
    class="rounded-md" 
    delimiter-icon="mdi-square" 
    height="350"
    hide-delimiters
    cycle>
      <v-carousel-item class="position-relative" v-for="(data, i) in info" :key="i" :src="images[i]" aspect-ratio="16/9"
        cover>
        <v-hover v-slot="{ props: hoverProps, isHovering }">
          <v-sheet 
          class="position-absolute bottom-0">
            <div class="d-flex fill-height justify-center align-center carouselText">
              <div class="text-h3 carrusel-text">
                {{ data }}
              </div>
            </div>
          </v-sheet>
        </v-hover>

      </v-carousel-item>

    </v-carousel>
  </v-card>

  
</template>


<script setup>

const images = [
  "https://cdn.pixabay.com/photo/2017/06/04/00/08/cebu-2370041_1280.jpg",
  "https://cdn.pixabay.com/photo/2016/05/21/04/17/bovine-1406354_1280.jpg",
  "https://media.istockphoto.com/id/1448347262/photo/herd-in-a-farm-corral.jpg?s=612x612&w=0&k=20&c=PBl6nFPTBy3QSZ9DGqF6O0hLip9mhZtFPVOpFFDeIng=",
]
const info = [
  'Descubre la manera más eficiente de gestionar tu finca con Herdix',
  'Identifica y agrega tus animales a tu base de datos',
  'Gestiona tus potreros y toma el control de tus espacios',
]

</script>

<style scoped>
.card-carousel{
  background: transparent !important;
  margin: 50px;
  background-color: #25632d;
}
.carousel {
  border-radius: 25px;
}

.carouselText {
  border-radius: 25px;

}

.carrusel-text{
  display: grid;
  justify-content: center;
  align-content: center;
  padding: 2%;
}




</style>