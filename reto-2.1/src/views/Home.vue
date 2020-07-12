<template>
  <div class="home">
      <Encabezado titulo="VIDEO PACHA TV"/>
      <CuerpoHome subtitulo="Lista de videos"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Encabezado from '@/components/Encabezado.vue'
import CuerpoHome from '@/components/CuerpoHome.vue'

export default {
  name: 'Home',
  components: {
    Encabezado,
    CuerpoHome
  }
}

</script>

<style lang="scss">

.Crud-CabeceraPrincipal {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color:  #ff5252;
  color: white;
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  box-shadow: 0px 10px 5px -4px rgba(196,196,196,1);
  padding: 2%;

  &-ModalAgregar {
    cursor: pointer;
    font-size: 1rem;
  }

  &-ModalAgregar:hover {
    color: black;
  }

}  

section header {
  padding: 0 2%;
  margin-bottom: 3%;
}

.Crud-ContenedorVideos {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
}

.Crud-CajaVideo {
  width: 22.5%;
  margin-bottom: 2%;
  margin-left: 2%;
  border: 1px solid #CFCFCF;

  &-Img {
    background-color: skyblue;
    border: none;
    width: 100%;
    height: 149px;
    margin-bottom: 0;
  }

  &-Contenido {
    padding: 0 4% 4% 4%;
   
    &-Visitas {
      font-size: .7rem;
    }

    &-Descripcion {
      font-size: .8rem;
    }

  }

  &-Contenido * {
    margin-top: 4%;
  }
}

.Crud-CajaVideo:hover {
  border: 1px solid #FF5252;
  box-shadow: 0px 0px 8px rgba(146, 146, 146, 0.53);
}

button {
  width: 100%;
  border: none;
  background: #00C1AA;
  box-shadow: 0px 0px 6px rgba(0, 0, 0, 0.25);
  color: white;
  font-size: .8rem;
  padding: 4% 0;
  text-align: center;
  cursor: pointer;
}

</style>
