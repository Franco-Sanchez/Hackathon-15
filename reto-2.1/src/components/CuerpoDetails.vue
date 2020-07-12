<template>
    <div class="cuerpoDetails">
        <section>
            <header>
                <h2>{{nombreVideo}}</h2>
            </header>
            <article class="VideoDetalle">
                <div class="VideoDetalle-Img"></div>
                <div class="VideoDetalle-Contenido">
                    <h3>{{nombreVideo}}</h3>
                    <p class="VideoDetalle-Contenido-Visitas">{{vistas}} visualizaciones</p>
                    <p class="VideoDetalle-Contenido-Detalle">Lorem ipsum dolor sit amet, consectetur adipiscing elit. A mauris morbi aliquam sollicitudin suspendisse feugiat. Et senectus eget nibh in. Nullam ullamcorper gravida viverra turpis aliquam at ac risus proin. Dignissim convallis risus, vestibulum et eget.</p>
                </div>
            </article>
        </section>
    </div>
</template>

<script>
export default {
    name: 'CuerpoDetails',
    props: {
        nombreVideo: {
            type: String,
            default: "Técnicas de programación"
        },
        vistas: {
            type: Number,
            default: 0
        }
    }
}
</script>