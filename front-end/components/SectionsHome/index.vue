<template>
  <v-app>
    <HomeInicio />
    <Footer />
  </v-app>
</template>

<script>
import Footer from '../components/Footer'
import HomeInicio from '../components/SectionsHome/Inicio'

export default {
  components: {
    Footer,
    HomeInicio,
  },
}
</script>
