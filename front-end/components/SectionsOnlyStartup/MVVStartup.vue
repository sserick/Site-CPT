<template>
  <v-container-fluid class="MVVStartupColor">
    <v-row justify="center" align="center">
      <v-col xs="12" md="4" class="SpacePadd" align="center">
        <v-row align="center" justify="center">
          <v-card class="MVVColor" flat>
            <v-img
              contain
              src="/imagens/Planetas/marte.png"
              class="PlanetSize"
            ></v-img>
            <h2 class="TituloMVVOne">Missão</h2>
          </v-card>
        </v-row>
      </v-col>
      <v-col xs="12" md="4" class="SpacePadd" align="center">
        <h4>Missão</h4>
      </v-col>
      <v-col xs="12" md="4" align="center" class="SpacePadd">
        <h4>Missão</h4>
      </v-col>
    </v-row>
    <v-row justify="center" align="center">
      <v-col xs="12" md="4" align="center" class="SpacePadd"> </v-col>
    </v-row>
  </v-container-fluid>
</template>

<script>
export default {
  props: {},
  data: () => ({
    overlay: false,
  }),
}
</script>

<style scoped>
.SpacePadd {
  padding: 0px;
  height: 100px;
}

.cardView {
  background-color: grey;
}

.cardItem {
  justify: center;
  align: center;
}

.spaceView {
  padding-bottom: 3%;
}

.spaceText {
  padding-left: 2%;
  padding-right: 2%;
}

.margin {
  margin-top: 27px;
}

.MVVStartupColor {
  background-color: #494b64;
}

.PlanetSize {
  width: 300px;
  height: 150px;
}
</style>
