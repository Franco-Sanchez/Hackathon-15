<template>
    <div class="details">
        <Encabezado titulo="VIDEO TV" />
        <CuerpoDetails />
    </div>
</template>

<script>

import Encabezado from '@/components/Encabezado.vue'
import CuerpoDetails from '@/components/CuerpoDetails.vue'

export default {
    name: 'Details',
    components: {
        Encabezado,
        CuerpoDetails
    }
}
</script>

<style lang="scss">

.VideoDetalle {
    padding: 0 2% 0 2%;

    &-Img {
        width: 100%;
        background-color: skyblue;
        height: 400px;
    }

    &-Contenido {

        &-Visitas {
            font-size: .7rem;
        }
        
        &-Detalle {
            color: #808080;
        }
    }

    &-Contenido * {
        margin-top: 1%;
    }
}
    
</style>