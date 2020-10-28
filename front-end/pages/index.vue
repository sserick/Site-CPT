<template>
  <v-app>
    <HomeInicio />
    <CarrosselNoticias />
    <MVV />
    <Visitas />
    <HomeSobreNos />
    <StartupExpirence />
    <Footer />
  </v-app>
</template>

<script>
import Footer from '../components/Footer'
import HomeInicio from '../components/SectionsHome/Inicio'
import HomeSobreNos from '../components/SectionsHome/SobreNos'
import MVV from '../components/SectionsHome/MVV'
import CarrosselNoticias from '../components/SectionsHome/CarrosselNoticias'
import StartupExpirence from '../components/SectionsHome/StartupExpirence'
import Visitas from '../components/SectionsHome/Visitas'

export default {
  components: {
    Footer,
    HomeSobreNos,
    HomeInicio,
    MVV,
    CarrosselNoticias,
    StartupExpirence,
    Visitas,
  },
}
</script>
