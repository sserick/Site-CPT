<template>
  <v-app>
    <initial />
    <pageVisits />
  </v-app>
</template>

<script>
import initial from '../components/SectionsHome/Inicio.vue'
import pageVisits from '../components/SectionsVisits/PageVisits.vue'

export default {
  components: {
    initial,
    pageVisits,
  },
  methods: {},
}
</script>

<style scoped></style>
