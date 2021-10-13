<template>
  <v-app>
    <navbar />
    <nuxt></nuxt>
    <footerSection />
  </v-app>
</template>

<script>
import navbar from '../components/navbar.vue'
import footerSection from '../components/footer.vue'

export default {
  components: {
    navbar,
    footerSection,
  },
}
</script>
