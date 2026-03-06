<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    p.mb-4 El siguiente mapa conceptual integra los criterios y especificidades de los conocimientos expuestos en el presente componente formativo.

    .row.justify-content-center
      .col-lg-12.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis.svg", alt="A continuación, se presenta la síntesis del componente formativo: Los modelos matemáticos y estadísticos aplicados al Big Data, los cuales constan de: Big data: datos estructurados, características, datos semiestructurados. Paquetes ofimáticos aplicados al modelado de datos: sistema de gestión lógica, herramientas tecnológicas. Técnicas de toma de decisiones: herramientas, modelos e instrumentos y finalmente los tipos. Estadística inferencial: muestra, población. Analítica de datos: teniendo acá la estadística descriptiva (tabla de frecuencia, gráficos, histograma) y los modelos matemáticos (uso, clasificación).")
      .col-auto
        a.anexo.mb-4(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis              

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
