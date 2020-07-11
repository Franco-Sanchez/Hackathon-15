<template>
    <div class="details">
        <header class="Crud-CabeceraPrincipal">
            <HelloWorld msg="VIDEO TV"/> 
            <HelloWorld class="Crud-CabeceraPrincipal-ModalAgregar" option="Ver mapa" />
        </header>
        <section>
            <header>
                <HelloWorld subtitulo="Tecnicas de programacion" />
            </header>
            <article>
                <div class="img"></div>
            </article>
        </section>
    </div>
</template>

<script>

import HelloWorld from '@/components/HelloWorld.vue'

export default {
    name: 'Details',
    components: {
        HelloWorld
    }
}
</script>

<style scoped lang="scss">

article {
    padding: 0 2% 0 2%;

    & .img {
        width: 100%;
        background-color: skyblue;
        height: 400px;
    }
}
    
</style>