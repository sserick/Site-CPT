<template>
  <v-container class="StartupColor">
    <v-row justify="center">
      <v-col cols="8">
        <v-card color="#230c3d">
          <v-img
            src="https://cdn.vuetifyjs.com/images/cards/house.jpg"
            class="white--text align-end"
            gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="400px"
          >
            <v-card-title>{{ name }}</v-card-title>
          </v-img>

          <v-card-actions class="justify-center">
            <v-card-text class="d-none d-md-block">{{ text }}</v-card-text>

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
.StartupColor {
  background-color: #10041c;
}

.colorExpansion {
  background-color: #230c3d;
}

a {
  text-decoration: none;
  color: white;
}
</style>
