<template>
  <v-card
    :loading="loading"
    class="mx-auto my-6"
    max-width="400"
    color="#3fa944"
  >
    <template slot="progress">
      <v-progress-linear
        color="yellow"
        height="10"
        indeterminate
      ></v-progress-linear>
    </template>

    <v-img
      height="150"
      src="https://cdn.vuetifyjs.com/images/cards/cooking.png"
    ></v-img>

    <v-card-title class="title">Nome do Evento</v-card-title>

    <v-card-text>
      <div class="my-4 subtitle-1">
        Gratuito
      </div>

      <div>
        Small plates, salads & sandwiches - an intimate setting with 12 indoor
        seats plus patio seating. Small plates, salads & sandwiches - an
        intimate setting with 12 indoor seats plus patio seating. Small plates,
        salads & sandwiches - an intimate setting with 12 indoor seats plus
        patio seating.
      </div>
    </v-card-text>

    <v-divider class="mx-4"></v-divider>

    <v-card-title>Data e horário</v-card-title>

    <v-card-text>
      <v-chip-group v-model="selection" color="black lighten-5" column>
        <v-chip color="yellow">14/10 - 5:30PM</v-chip>

        <v-chip color="yellow">15/10 - 7:30PM</v-chip>

        <v-chip color="yellow">18/10 - 8:00PM</v-chip>

        <v-chip color="yellow">19/10 - 9:00PM</v-chip>
      </v-chip-group>
    </v-card-text>

    <v-card-actions class="buttonsEvent">
      <v-btn color="white lighten-2" text @click="reserve">
        Inscreva-se
      </v-btn>
      <v-btn color="white lighten-2" text @click="reserve">
        Saiba mais
      </v-btn>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {
  props: {},
  data() {
    return {
      loading: false,
      selection: 1,
    }
  },

  methods: {
    reserve() {
      this.loading = true

      setTimeout(() => (this.loading = false), 2000)
    },
  },
}
</script>

<style scoped>
.EventColor {
  background-color: #3fa944;
}

.title {
  color: #fcd24a;
}

.EventColorOne {
  background-color: #3fa944;
}

.buttonsEvent {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
</style>
