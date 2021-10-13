<template>
  <container>
    <footerInsta />
    <footerGeral />
  </container>
</template>

<script>
import footerInsta from '../components/FooterItens/FooterInstagram.vue'
import footerGeral from '../components/FooterItens/FooterDescription.vue'

export default {
  components: {
    footerInsta,
    footerGeral,
  },
}
</script>

<style scoped></style>
