<template>
  <v-app>
    <Inicio titulo="Sobre Nós" />
    <SobreNosTexto />
    <Footer />
  </v-app>
</template>

<script>
import Footer from '../components/Footer'
import Inicio from '../components/Inicio'
import SobreNosTexto from '../components/SectionsSobreNos/SobreNosTexto'

export default {
  components: {
    Footer,
    Inicio,
    SobreNosTexto,
  },
  methods: {},
}
</script>

<style scoped></style>
