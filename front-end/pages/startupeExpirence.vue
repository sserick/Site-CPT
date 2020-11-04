<template>
  <v-app>
    <Inicio titulo="Startup Expirence" />
    <StartupExpirenceTexto />
    <Footer />
  </v-app>
</template>

<script>
import Footer from '../components/Footer'
import Inicio from '../components/Inicio'
import StartupExpirenceTexto from '../components/SectionsStartupExpirence/StartupExpirenceTexto'

export default {
  components: {
    Footer,
    Inicio,
    StartupExpirenceTexto
  },
  methods: {}
}
</script>

<style scoped></style>
