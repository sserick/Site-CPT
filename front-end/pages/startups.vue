<template>
  <v-app>
    <Inicio titulo="Startups" />
    <v-container-fluid class="marginTop">
      <v-row>
        <v-col v-for="item in startups" :key="item.name" cols="12">
          <Startup :name="item.name" :text="item.text" :href="item.href" />
        </v-col>
      </v-row>
    </v-container-fluid>
    <Footer />
  </v-app>
</template>

<script>
import Footer from '../components/Footer'
import Inicio from '../components/Inicio'
import Startup from '../components/SectionsStartups/Startup'

export default {
  components: {
    Footer,
    Inicio,
    Startup,
  },
  data() {
    return {
      startups: [
        {
          name: 'Nome da Startup 1',
          text:
            'Small plates, salads & sandwiches - an intimate setting with 12 indoor Small plates, salads & sandwiches - an intimate setting with 12 indoor Small plates, salads & sandwiches - an intimate setting with 12 indoor',
          href: '',
          imagem: '',
        },
        {
          name: 'Nome da Startup 2',
          text:
            'Small plates, salads & sandwiches - an intimate setting with 12 indoor Small plates, salads & sandwiches - an intimate setting with 12 indoor Small plates, salads & sandwiches - an intimate setting with 12 indoor',
          href: '',
          imagem: '',
        },
        {
          name: 'Nome da Startup 3',
          text:
            'Small plates, salads & sandwiches - an intimate setting with 12 indoor Small plates, salads & sandwiches - an intimate setting with 12 indoor Small plates, salads & sandwiches - an intimate setting with 12 indoor',
          href: '',
          imagem: '',
        },
      ],
    }
  },
  methods: {},
}
</script>

<style scoped>
.marginTop {
  padding-top: 5%;
  padding-bottom: 5%;
  background-color: #10041c;
}
</style>
