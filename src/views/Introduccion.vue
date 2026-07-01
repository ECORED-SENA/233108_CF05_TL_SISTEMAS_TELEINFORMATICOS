<template lang="pug">
  .curso-main-container.introduccion
    BannerInterno
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
      .titulo-principal.color-acento-contenido(data-aos="flip-up")
        .titulo-principal__numero
          span
            i.fas.fa-info
        h1 Introducción
      .row.justify-content-center.align-items-center.mb-4(data-aos="fade-right")
        .bloque-texto-g.color-primario.p-3.p-sm-4.p-md-5
          .bloque-texto-g__img(
            :style="{ backgroundImage: `url(${require_src('@/assets/curso/temas/intro/img1.png')})` }")
          .bloque-texto-g__texto.p-4
            p.mb-0 Antes de adentrarse en el diseño de una red computacional, es fundamental establecer una clara comprensión de su naturaleza. En tiempos pasados, el término "red" se refería simplemente a un conjunto de líneas en serie que conectaban terminales poco inteligentes a computadoras centrales. Otros ejemplos destacados incluían la red telefónica de voz y la red de televisión por cable, diseñadas para transmitir señales de vídeo. Estas redes tienen en común su especialización en el manejo de un tipo específico de datos (tales como pulsaciones, voz o vídeo) y su conexión a dispositivos diseñados con un propósito particular, como terminales, receptores manuales y televisores.
      p.mb-4(data-aos="fade-left") Por tanto, para comprender verdaderamente la complejidad de diseñar una red de este tipo, resulta imperativo reflexionar sobre su relevancia y papel en la actualidad. El siguiente video introductorio ofrece una plataforma para meditar acerca de la importancia y el papel en constante evolución que desempeñan las redes computacionales en nuestro mundo contemporáneo.
      .row.justify-content-center.align-items-center(data-aos="fade-right")
        figure
          .video
            iframe(width="560" height="315" src="https://www.youtube.com/embed/jSS_7XYl50w" title="Comunicación de marketing digital" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
          figcaption Video. Comunicación de marketing digital

</template>

<script>
export default {
  name: 'Introduccion',
  data: () => ({
    // variables de vue
  }),
}
</script>

<style lang="sass"></style>
