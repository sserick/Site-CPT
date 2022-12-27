<template>
  <v-container fluid class="sectionMVV">
    <v-row align="start" justify="center">
      <v-spacer class="d-none d-lg-flex" />
      <v-col cols="10" md="5" sm="5" lg="3">
        <v-row justify="center" align="center">
          <v-icon class="IconPageMVV" size="70">mdi-flask-outline</v-icon>
        </v-row>
        <v-row justify="center" align="center">
          <h2 class="TitlePageMVV">MISSÃO</h2>
        </v-row>
        <v-row justify="center" align="center">
          <p class="TextPageMVV">
            Reunir e desenvolver capacitação profissional, objetivando a
            democratização do conhecimento e aproximando a universidade do
            mercado. Trabalhar em um ambiente de co-working, buscando soluções
            inovadoras para a sociedade.
          </p>
        </v-row>
      </v-col>
      <v-spacer class="d-none d-lg-flex" />
      <v-col cols="10" md="5" sm="5" lg="3">
        <v-row justify="center" align="center">
          <v-icon class="IconPageMVV" size="70">mdi-rocket</v-icon>
        </v-row>
        <v-row justify="center" align="center">
          <h2 class="TitlePageMVV">VISÃO</h2>
        </v-row>
        <v-row justify="center" align="center">
          <p class="TextPageMVV">
            Ser reconhecido como projeto de referência em inovação, extensão e
            tecnologia. Nossa reputação será construída com soluções
            inteligentes e inovadoras, visando sempre a transferência de
            tecnologia.
          </p>
        </v-row>
      </v-col>
      <v-spacer class="d-none d-lg-flex" />
      <v-col cols="10" md="5" sm="5" lg="3">
        <v-row justify="center" align="center">
          <v-icon class="IconPageMVV" size="70">mdi-dna</v-icon>
        </v-row>
        <v-row justify="center" align="center">
          <h2 class="TitlePageMVV">VALORES</h2>
        </v-row>
        <v-row justify="center" align="center" class="rowVal">
          <p class="textVal">
            Inovação, interdisciplinaridade, Foco no resultado, autonomia,
            disciplina, comunicação, teamwork, dedicação, ciência, sentimento de
            pertencimento.
          </p>
        </v-row>
      </v-col>
      <v-spacer class="d-none d-lg-flex" />
    </v-row>
  </v-container>
</template>

<script>
export default {}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300&display=swap');

.sectionMVV {
  padding-top: 4%;
  padding-bottom: 4%;
  background-color: #3fa944;
}

.TitlePageMVV {
  font-size: 36px;
  font-family: 'Open Sans', sans-serif;
  text-align: left;
  color: white;
  font-weight: bold;
  margin-bottom: 30px;
}

.TextPageMVV {
  font-size: 15px;
  font-family: 'Open Sans', sans-serif;
  text-align: justify;
  color: black;
}

.textVal {
  font-size: 15px;
  font-family: 'Open Sans', sans-serif;
  text-align: justify;
  color: black;
  width: 100%;
  margin-bottom: 0px;
}

.IconPageMVV {
  font-size: 36px;
  font-family: 'Open Sans', sans-serif;
  text-align: left;
  color: white;
  font-weight: 900;
  padding: 30px;
  border-color: white;
  border-width: 2px;
  border-style: solid;
  border-radius: 90px;
  margin-bottom: 30px;
}

.IconPageMVV:hover {
  border-color: white;
  color: #3fa944;
  background-color: white;
}

.TitleValores {
  font-size: 36px;
  font-family: 'Open Sans', sans-serif;
  text-align: center;
  color: black;
  font-weight: 900;
}

@media (max-width: 767px) {
  .TextPageMVV {
    height: 170px;
  }
}
</style>
