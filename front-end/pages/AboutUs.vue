<template>
  <v-app>
    <initial />
    <aboutUsInfo />
  </v-app>
</template>

<script>
import initial from '../components/SectionsHome/Inicio.vue'
import aboutUsInfo from '../components/SectionsAboutUs/AboutUsInfo.vue'

export default {
  components: {
    initial,
    aboutUsInfo,
  },
  methods: {},
}
</script>

<style scoped></style>
