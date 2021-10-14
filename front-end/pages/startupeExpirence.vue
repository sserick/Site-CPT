<template>
  <v-app>
    <initial />
    <startupExpirenceInfo />
  </v-app>
</template>

<script>
import initial from '../components/SectionsHome/Inicio.vue'
import startupExpirenceInfo from '../components/SectionsStartupExpirence/StartupExpirenceInfo'

export default {
  components: {
    initial,
    startupExpirenceInfo,
  },
  methods: {},
}
</script>

<style scoped></style>
