<template>
  <v-app>
    <initial />
    <mvv />
    <visitas />
    <startupeExpirence />
  </v-app>
</template>

<script>
import startupeExpirence from '../components/SectionsHome/StartupExpirence.vue'
import visitas from '../components/SectionsHome/Visitas.vue'
import initial from '../components/SectionsHome/Inicio.vue'
import mvv from '../components/SectionsHome/MVV.vue'

export default {
  components: {
    initial,
    mvv,
    visitas,
    startupeExpirence,
  },
}
</script>
