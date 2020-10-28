<template>
  <v-card
    :loading="loading"
    class="mx-auto my-12"
    max-width="574"
    color="#230c3d"
  >
    <template slot="progress">
      <v-progress-linear
        color="yellow"
        height="10"
        indeterminate
      ></v-progress-linear>
    </template>

    <v-img
      height="250"
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
      <v-chip-group v-model="selection" color="purple lighten-5" column>
        <v-chip color="purple">14/10 - 5:30PM</v-chip>

        <v-chip color="purple">15/10 - 7:30PM</v-chip>

        <v-chip color="purple">18/10 - 8:00PM</v-chip>

        <v-chip color="purple">19/10 - 9:00PM</v-chip>
      </v-chip-group>
    </v-card-text>

    <v-card-actions>
      <v-btn color="yellow lighten-2" text @click="reserve">
        Inscreva-se
      </v-btn>
      <v-btn color="yellow lighten-2" text @click="reserve">
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
      selection: 1
    }
  },

  methods: {
    reserve() {
      this.loading = true

      setTimeout(() => (this.loading = false), 2000)
    }
  }
}
</script>

<style scoped>
.EventColor {
  background-color: #10041c;
}

.title {
  color: #fcd24a;
}

.EventColorOne {
  background-color: #151626;
}
</style>
