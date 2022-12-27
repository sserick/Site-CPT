<template>
  <v-app>
    <initial />
    <v-container fluid class="EventColor">
      <v-row justify="center" align="center">
        <v-col cols="12">
          <h1 class="TitleEvents">Em andamento</h1>
        </v-col>
        <v-col
          v-for="(evento, i) in InProgress"
          :key="i"
          cols="10"
          sm="10"
          md="4"
          lg="4"
        >
          <events />
        </v-col>
      </v-row>
      <v-row justify="center" align="center" class="Pagination">
        <v-col cols="10" md="10" lg="5" xl="5">
          <v-row justify="center" align="center">
            <v-pagination
              v-model="pageProgress"
              color="#3fa944"
              :length="6"
              circle
            ></v-pagination>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
    <v-container fluid class="EventColor">
      <v-row justify="center" align="center">
        <v-col cols="12">
          <h1 class="TitleEvents">Próximos Eventos</h1>
        </v-col>
        <v-col
          v-for="(evento, i) in Next"
          :key="i"
          cols="10"
          sm="10"
          md="4"
          lg="4"
        >
          <events />
        </v-col>
      </v-row>
      <v-row justify="center" align="center" class="Pagination">
        <v-col cols="10" md="10" lg="5" xl="5">
          <v-row justify="center" align="center">
            <v-pagination
              v-model="pageNext"
              color="#3fa944"
              :length="6"
              circle
            ></v-pagination>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
    <v-container fluid class="EventColor">
      <v-row justify="center" align="center">
        <v-col cols="12">
          <h1 class="TitleEvents">Realizados</h1>
        </v-col>
        <v-col
          v-for="(evento, i) in finalized"
          :key="i"
          cols="10"
          sm="10"
          md="4"
          lg="4"
        >
          <events />
        </v-col>
      </v-row>
      <v-row justify="center" align="center" class="Pagination">
        <v-col cols="10" md="10" lg="5" xl="5">
          <v-row justify="center" align="center">
            <v-pagination
              v-model="pageFinalized"
              color="#3fa944"
              :length="6"
              circle
            ></v-pagination>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<script>
import initial from '../components/SectionsHome/Inicio.vue'
import events from '../components/SectionsEvents/Event.vue'

export default {
  components: {
    initial,
    events,
  },
  data() {
    return {
      pageProgress: 1,
      pageNext: 1,
      pageFinalized: 1,
      InProgress: [
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
      Next: [
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
      finalized: [
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
  background-color: RGBA(63, 169, 68, 0.05);
  padding-top: 3%;
  padding-left: 5%;
  padding-right: 5%;
}

.TitleEvents {
  text-align: left;
  font-size: 36px;
  font-weight: 900;
  font-family: 'Open Sans', sans-serif;
  color: #3fa944;
}
</style>
