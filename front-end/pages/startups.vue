<template>
  <v-app>
    <initial />
    <v-container-fluid class="marginTop">
      <v-row justify="center" align="center">
        <v-col
          v-for="item in startups"
          :key="item.name"
          cols="6"
          class="padding"
        >
          <startup :name="item.name" :text="item.text" :href="item.href" />
        </v-col>
      </v-row>
    </v-container-fluid>
  </v-app>
</template>

<script>
import initial from '../components/SectionsHome/Inicio.vue'
import startup from '../components/SectionsStartups/Startup'

export default {
  components: {
    initial,
    startup,
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
        {
          name: 'Nome da Startup 4',
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
  background-color: RGBA(63, 169, 68, 0.05);
}

.padding {
  padding: 0px;
}
</style>
