<template>
  <v-container-fluid class="MVVColor margin">
    <v-row align="center" justify="center">
      <v-col align="center" cols="12" sm="3">
        <v-row align="center" justify="center" class="MVVColor">
          <v-card class="MVVColor" flat>
            <v-img
              contain
              src="/imagens/Planetas/marte.png"
              class="PlanetSize"
              @mouseover="hoverOne = true"
              @mouseleave="hoverOne = false"
            ></v-img>
            <h2 class="TituloMVVOne">Missão</h2>
          </v-card>
        </v-row>
      </v-col>
      <v-col align="center" cols="12" sm="3">
        <v-row align="center" justify="center" class="MVVColor">
          <v-card class="MVVColor" flat>
            <v-img
              contain
              src="/imagens/Planetas/urano.png"
              class="PlanetSize"
              @mouseover="hoverTwo = true"
              @mouseleave="hoverTwo = false"
            ></v-img>
            <h2 class="TituloMVVOne">Visão</h2>
          </v-card>
        </v-row>
      </v-col>
      <v-col align="center" cols="12" sm="3">
        <v-row align="center" justify="center" class="MVVColor">
          <v-card class="MVVColor" flat>
            <v-img
              contain
              src="/imagens/Planetas/venus.png"
              class="PlanetSize"
              @mouseover="hoverTree = true"
              @mouseleave="hoverTree = false"
            ></v-img>
            <h2 class="TituloMVVOne">Valores</h2>
          </v-card>
        </v-row>
      </v-col>
    </v-row>
    <v-row class="MarginTextoMVV">
      <v-col v-if="hoverOne" cols="1" sm="3" class="TextoMVV"></v-col>
      <v-col v-if="hoverOne" cols="10" sm="6" class="TextoMVV">
        <span class="TextoMVVOne">
          Reunir e desenvolver capacitação profissional, objetivando a
          democratização do conhecimento e aproximando a universidade do
          mercado. Trabalhar em um ambiente de co-working, buscando soluções
          inovadoras para a sociedade.
        </span>
      </v-col>
      <v-col v-if="hoverOne" cols="1" sm="3" class="TextoMVV"></v-col>
    </v-row>
    <v-row>
      <v-col v-if="hoverTwo" cols="1" sm="3" class="TextoMVV"></v-col>
      <v-col v-if="hoverTwo" cols="10" sm="6" class="TextoMVV">
        <span class="TextoMVVOne">
          Ser reconhecido como projeto de referência em inovação, extensão e
          tecnologia. Nossa reputação será construída com soluções inteligentes
          e inovadoras, visando sempre a transferência de tecnologia.
        </span>
      </v-col>
      <v-col v-if="hoverTwo" cols="1" sm="3" class="TextoMVV"></v-col>
    </v-row>
    <v-row class="MVVColor">
      <v-col v-if="hoverTree" cols="1" sm="3" class="TextoMVV"></v-col>
      <v-col v-if="hoverTree" cols="10" sm="6" class="TextoMVV">
        <span class="TextoMVVOne">
          Inovação, interdisciplinaridade, Foco no resultado, autonomia,
          disciplina, comunicação, teamwork, dedicação, ciência, sentimento de
          pertencimento.
        </span>
      </v-col>
      <v-col v-if="hoverTree" cols="1" sm="3" class="TextoMVV"></v-col>
    </v-row>
  </v-container-fluid>
</template>

<script>
export default {
  data() {
    return {
      hoverOne: false,
      hoverTwo: false,
      hoverTree: false,
    }
  },
}
</script>

<style scoped>
.margin {
  padding-top: 20px;
}

.PlanetSize {
  width: 200px;
  height: 200px;
}

.PlanetSize:hover {
  transform: rotate(300deg);
}

.PlanetSize {
  transform: rotate(55deg);
  transition: transform 3s;
}

.TextoMVV {
  background-color: #230c3d;
  height: 300px;
  display: flex;
  flex-direction: row;
  align-items: center;
}

.TextoMVVOne {
  color: #fff;
  font-family: 'Arapey', 'Montserrat';
  text-align: center;
  font-size: 20px;
}

.TituloMVVOne {
  margin-top: 10px;
  color: #fff;
  font-family: 'Arapey', 'Montserrat';
  font-size: 20px;
}

.MarginTextoMVV {
  margin-top: 40px;
}

.MVVColor {
  background-color: #10041c;
}

@media screen and (max-width: 464px) {
  .PlanetSize {
    width: 100px;
    height: 100px;
  }
}

@media (min-width: 465px) and (max-width: 700px) {
  .PlanetSize {
    width: 110px;
    height: 110px;
  }
}

@media (min-width: 701px) and (max-width: 958px) {
  .PlanetSize {
    width: 150px;
    height: 150px;
  }
}
</style>
