<template>
  <v-container-fluid class="FluxogramaColor spaceView">
    <v-row justify="center" align="center">
      <v-col xs="10" md="10" align="center">
        <h2 class="black--text marginText">Fluxograma</h2>
        <p class="black--text">
          Desde a fundação do NPDEAS os coordenadoras realizam atividades como
          visitas dirigidas aos laboratórios do grupo de pesquisa. Várias
          escolas e universidades do Brasil e do Mundo passaram pelos
          laboratórios e conheceram as pesquisas realizadas na UFPR com foco em
          Energia Renovável, Biotecnologia e Meio Ambiente.
        </p>
      </v-col>
      <v-col xs="10" md="10" align="center">
        <v-img src="/imagens/HomeFoto.JPG" class="ImageSize justify-end">
        </v-img>
      </v-col>
    </v-row>
  </v-container-fluid>
</template>

<script>
export default {}
</script>

<style>
.marginText {
  padding-bottom: 2%;
}

.ImageSize {
  height: 700px;
  width: 1200px;
}

.FluxogramaColor {
  background-color: #ffffff;
}

.spaceView {
  padding-top: 3%;
  padding-bottom: 3%;
}
</style>
