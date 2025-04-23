<template>
  <div class="empanada">

    <div class="seccion">
      <img 
        :width="400"
        aspect-ratio="16/9" 
        class="logo" 
        src="/public/HERDIX-LOGO-copia.svg"
      >
    </div>

    <div class="seccion">
      <p class="text-center text-h2">
        ¡Descubre la forma más fácil y eficiente de administrar tu finca con Herdix!
      </p>
    </div>

  </div>
</template>

<style scoped lang="scss">
  p{
    color: white;
  }
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
    // background: #25632d;
    background-color: $verdeHerdixOscuro;
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