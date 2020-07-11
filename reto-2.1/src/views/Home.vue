<template>
  <div class="home">
    <article>
      <header class="Crud-CabeceraPrincipal">
        <HelloWorld msg="VIDEO PACHA TV"/>
        <HelloWorld class="Crud-CabeceraPrincipal-ModalAgregar" option="Agregar Video" />
      </header>
      <section>
        <header>
          <HelloWorld subtitulo="Lista de videos"/>
        </header>
        <article class="Crud-ContenedorVideos">
          <div class="Crud-CajaVideo">
            <div class="Crud-CajaVideo-Img"></div>
            <div class="Crud-CajaVideo-Contenido">
              <h3>Tecnicas de programación</h3>
              <p class="Crud-CajaVideo-Contenido-Visu">0 visualizaciones</p>
              <p class="Crud-CajaVideo-Contenido-Descripcion">Lorem ipsum dolor sit amet, consectetur adipiscing elit. A mauris morbi aliquam sollicitudin suspendisse feugiat. Et senectus eget nibh in. Nullam ullamcorper gravida viverra turpis aliquam at ac risus proin. Dignissim convallis risus, vestibulum et eget.</p>
              <router-link to="/details"><div>Ver detalle</div></router-link>
            </div>
          </div>
        </article>
      </section>     
    </article>            
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
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
  }

  &-ModalAgregar:hover {
    color: black;
  }

}  

h1 {
  font-size: 2.2rem;
}

h2 {
  font-size: 1.8rem;
  font-weight: bold;
}

section {
  margin-top: 3%;
  margin-bottom: 3%;
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

    & h3 {
      font-size: .9rem;
      font-weight: bold;
    }

    &-Visu {
      font-size: .7rem;
    }

    &-Descripcion {
      font-size: .8rem;
    }

    /* &-a {
      width: 100%;
      border: none;
      background: #00C1AA;
      box-shadow: 0px 0px 6px rgba(0, 0, 0, 0.25);
      color: white;
      font-size: .8rem;
      padding: 4% 0;
      } */
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
  cursor: pointer;
}

a {
  text-decoration: none;
}

a div {
  width: 100%;
  border: none;
  background: #00C1AA;
  box-shadow: 0px 0px 6px rgba(0, 0, 0, 0.25);
  color: white;
  font-size: .8rem;
  padding: 4% 0;
  text-align: center;
}

</style>
