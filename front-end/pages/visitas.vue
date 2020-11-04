<template>
  <v-app>
    <Inicio titulo="Visitas" />
    <VisitasTexto />
    <Footer />
  </v-app>
</template>

<script>
import Footer from '../components/Footer'
import Inicio from '../components/Inicio'
import VisitasTexto from '../components/SectionsVisitas/VisitasTexto'

export default {
  components: {
    Footer,
    Inicio,
    VisitasTexto,
  },
  methods: {},
}
</script>

<style scoped></style>
