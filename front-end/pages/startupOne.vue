<template>
  <v-app>
    <InicioStartup />
    <MVVStartup />
    <SobreNos />
    <SuporteAtividadesStartup />
    <FluxogramaStartup />
  </v-app>
</template>

<script>
import InicioStartup from '../components/SectionsOnlyStartup/InicioStartup'
import MVVStartup from '../components/SectionsOnlyStartup/MVVStartup'
import SobreNos from '../components/SectionsOnlyStartup/SobreNosStartup'
import SuporteAtividadesStartup from '../components/SectionsOnlyStartup/SuporteAtividadesStartup'
import FluxogramaStartup from '../components/SectionsOnlyStartup/FluxogramaStartup'

export default {
  components: {
    InicioStartup,
    MVVStartup,
    SobreNos,
    SuporteAtividadesStartup,
    FluxogramaStartup,
  },
  data() {
    return {}
  },
  methods: {},
}
</script>

<style scoped></style>
