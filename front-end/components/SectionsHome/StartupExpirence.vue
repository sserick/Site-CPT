<template>
  <v-container-fluid class="visitas-bg">
    <v-row justify="center" align="center">
      <v-col cols="12" lg="6" class="image"> </v-col>
      <v-col cols="12" lg="6">
        <v-row justify="center" align="center" class="textGeral">
          <v-col cols="12">
            <h4 class="VisitasTitle">Startup Expirience</h4>
          </v-col>
          <v-col cols="12">
            <p class="VisitasText">
              Desde a fundação do NPDEAS os coordenadoras realizam atividades
              como visitas dirigidas aos laboratórios do grupo de pesquisa.
              Várias escolas e universidades do Brasil e do Mundo passaram pelos
              laboratórios e conheceram as pesquisas realizadas na UFPR com foco
              em Energia Renovável, Biotecnologia e Meio Ambiente. Agora, a
              partir de Agosto de 2016, o NPDEAS conta com o Projeto de Extensão
              Universitária destinado divulgação da Ciência, Tecnologia e
              Inovação para a Sociedade. Trata-se do CIÊNCIA PARA TODOS que tem
              como público alvo alunos, funcionários e professores de escolas do
              ensino fundamental, médio e profissional. O projeto contará com o
              envolvimento de professores e alunos da UFPR responsáveis pela
              realização das atividades ao público alvo. Neste projeto haverá o
              envolvimento dos alunos da graduação que vão receber capacitação
              para realizar as atividades propostas de divulgação da Ciência
              para a comunidade. Assim como o NPDEAS, este projeto de extensão é
              essencialmente interdisciplinar e vai contar inicialmente com
              alunos de graduação de diversas áreas da Universidade como, por
              exemplo, os cursos de Biotecnologia, Biologia, Engenharia Química,
              Engenharia Elétrica, Engenharia Mecânica e Engenharia Florestal. O
              NPDEAS entende que o desenvolvimento de Ciência e Tecnologia é
              estratégico para o desenvolvimento de um país. A inovação de
              produtos, processos ou modelos de negócio podem catalisar as
              modificações necessárias para a melhoria econômica de uma nação e
              alavancar o aumento sustentável da qualidade de vida da população.
              As universidades compõem o celeiro do desenvolvimento científico e
              tecnológico e, desta forma, são os atores com capacidade de
              iniciar essa transformação.
            </p>
          </v-col>
        </v-row>
        <v-row justify="center" align="stretch" class="button">
          <v-col cols="12" class="buttonAling">
            <v-btn
              large
              rounded
              color="#3fa944"
              class="white--text"
              href="/startupeExpirence"
            >
              Saiba mais
              <v-icon right dark>mdi-rocket</v-icon>
            </v-btn>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container-fluid>
</template>

<script>
export default {}
</script>

<style scoped>
.visitas-bg {
  background-color: white;
}

.image {
  height: 750px;
  background-image: url('/imagens/visita.JPG');
  background-repeat: no-repeat;
  background-size: cover;
  padding: 0;
}

.button {
  padding-left: 10%;
  padding-right: 10%;
}

.buttonAling {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.VisitasTitle {
  color: #3fa944;
  text-align: center;
  font-size: 35px;
  padding-top: 5%;
}

.VisitasText {
  text-align: justify;
  font-size: 14px;
  color: black;
  padding-left: 10%;
  padding-right: 10%;
}

.alignButton {
  display: flex;
  flex-direction: row;
  align-items: center;
  align-self: flex-end;
  margin-top: 10%;
}

.ImageSize {
  height: auto;
  width: auto;
}

@media screen and (max-width: 464px) {
  .ImageSize {
    height: 200px;
    width: 300px;
  }
}

@media (min-width: 465px) and (max-width: 700px) {
  .ImageSize {
    height: 300px;
    width: 400px;
  }
}

@media (min-width: 701px) and (max-width: 959px) {
  .ImageSize {
    height: 400px;
    width: 500px;
  }
}

@media (min-width: 960px) and (max-width: 1305px) {
}
</style>
