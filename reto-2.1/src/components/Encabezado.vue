<template>
  <div class="encabezado">
    <article>
      <header class="Crud-CabeceraPrincipal">
        <h1>{{titulo}}</h1>
        <p class="Crud-CabeceraPrincipal-ModalAgregar">{{btnAgregar}}</p>
      </header> 
    </article>  
  </div>
</template>

<script>
export default {
  name: 'Encabezado',
  props: {
    titulo: String,  
    btnAgregar: {
      type: String,
      default: "Agregar Video"
    }  
  }
}
</script>
