<template>
  <v-container fluid class="StartupColor">
    <v-row justify="center" align="center">
      <v-col cols="9">
        <v-card color="#3fa944">
          <v-img
            src="https://cdn.vuetifyjs.com/images/cards/house.jpg"
            class="white--text align-end"
            gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="300px"
          >
            <v-card-title>{{ name }}</v-card-title>
          </v-img>

          <v-card-actions class="justify-center">
            <v-card-text class="d-none d-md-block">{{ text }}</v-card-text>
          </v-card-actions>
          <v-card-actions class="justify-center">
            <v-btn
              :href="href"
              large
              rounded
              color="#fcd24a"
              class="black--text"
            >
              Saiba mais
              <v-icon right dark>mdi-rocket</v-icon>
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      required: true,
      default: 'Título',
    },
    text: {
      type: String,
      required: true,
      default: 'Texto da startup',
    },
    imagem: {
      type: String,
      default: '/imagens/Icons/LogoCPT.png',
    },
    href: {
      type: String,
      required: true,
      default: '/imagens/Icons/LogoCPT.png',
    },
  },
  data() {
    return {}
  },
}
</script>

<style>
a {
  text-decoration: none;
  color: white;
}
</style>
