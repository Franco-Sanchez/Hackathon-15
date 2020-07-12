<template>
    <div class="cuerpoHome">
        <section>
            <header>
                <h2>{{subtitulo}}</h2>
            </header>
            <article class="Crud-ContenedorVideos">
                <div class="Crud-CajaVideo">
                    <div class="Crud-CajaVideo-Img"></div>
                    <div class="Crud-CajaVideo-Contenido">
                        <h3>{{nombreVideo}}</h3>
                        <p class="Crud-CajaVideo-Contenido-Visitas">{{vistas}} visualizaciones</p>
                        <p class="Crud-CajaVideo-Contenido-Descripcion">Lorem ipsum dolor sit amet, consectetur adipiscing elit. A mauris morbi aliquam sollicitudin suspendisse feugiat. Et senectus eget nibh in. Nullam ullamcorper gravida viverra turpis aliquam at ac risus proin. Dignissim convallis risus, vestibulum et eget.</p>
                        <router-link to="/details"><button>Ver detalle</button></router-link>
                    </div>
                </div>
            </article>
        </section>
    </div>
</template>

<script>
export default {
    name: 'CuerpoHome',
    props: {
        subtitulo: String,
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