<template>
  <v-app>
    <Inicio titulo="Eventos" />
    <v-container-fluid class="EventColor">
      <v-row justify="center">
        <v-col
          v-for="(evento, i) in eventos"
          :key="i"
          cols="12"
          sm="12"
          md="5"
          lg="5"
        >
          <Events />
        </v-col>
      </v-row>
    </v-container-fluid>
    <Footer />
  </v-app>
</template>

<script>
import Footer from '../components/Footer'
import Inicio from '../components/Inicio'
import Events from '../components/SectionsEvents/Event'

export default {
  components: {
    Footer,
    Inicio,
    Events,
  },
  data() {
    return {
      eventos: [
        {
          title: 'Nome do Evento',
          image: '',
          pagamento: 'Gratuito',
          descrição: '',
          datahoraOne: '',
          datahoraTwo: '',
          datahoraTree: '',
          datahoraFour: '',
          linkForm: '',
          linkSaibaMais: '',
        },
        {
          title: 'Nome do Evento',
          image: '',
          pagamento: 'Gratuito',
          descrição: '',
          datahoraOne: '',
          datahoraTwo: '',
          datahoraTree: '',
          datahoraFour: '',
          linkForm: '',
          linkSaibaMais: '',
        },
        {
          title: 'Nome do Evento',
          image: '',
          pagamento: 'Gratuito',
          descrição: '',
          datahoraOne: '',
          datahoraTwo: '',
          datahoraTree: '',
          datahoraFour: '',
          linkForm: '',
          linkSaibaMais: '',
        },
        {
          title: 'Nome do Evento',
          image: '',
          pagamento: 'Gratuito',
          descrição: '',
          datahoraOne: '',
          datahoraTwo: '',
          datahoraTree: '',
          datahoraFour: '',
          linkForm: '',
          linkSaibaMais: '',
        },
      ],
    }
  },
  methods: {},
}
</script>

<style scoped>
.EventColor {
  background-color: #10041c;
  padding-top: 3%;
  padding-bottom: 3%;
}
</style>
