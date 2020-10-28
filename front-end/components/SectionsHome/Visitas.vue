<template>
  <v-container-fluid class="margin VisitasColor">
    <v-row justify="center" align="center">
      <v-col v-for="k in 2" :key="k" cols="12" lg="5" align="center">
        <v-card
          v-if="k === 1"
          class="VisitasColor paddingText"
          flat
          height="100%"
          width="700px"
        >
          <h4 class="VisitasTitle">Visitas</h4>
          <h5 class="VisitasText">
            Desde a fundação do NPDEAS os coordenadoras realizam atividades como
            visitas dirigidas aos laboratórios do grupo de pesquisa. Várias
            escolas e universidades do Brasil e do Mundo passaram pelos
            laboratórios e conheceram as pesquisas realizadas na UFPR com foco
            em Energia Renovável, Biotecnologia e Meio Ambiente. Agora, a partir
            de Agosto de 2016, o NPDEAS conta com o Projeto de Extensão
            Universitária destinado divulgação da Ciência, Tecnologia e Inovação
            para a Sociedade. Trata-se do CIÊNCIA PARA TODOS que tem como
            público alvo alunos, funcionários e professores de escolas do ensino
            fundamental, médio e profissional. O projeto contará com o
            envolvimento de professores e alunos da UFPR responsáveis pela
            realização das atividades ao público alvo. Neste projeto haverá o
            envolvimento dos alunos da graduação que vão receber capacitação
            para realizar as atividades propostas de divulgação da Ciência para
            a comunidade. Assim como o NPDEAS, este projeto de extensão é
            essencialmente interdisciplinar e vai contar inicialmente com alunos
            de graduação de diversas áreas da Universidade como, por exemplo, os
            cursos de Biotecnologia, Biologia, Engenharia Química, Engenharia
            Elétrica, Engenharia Mecânica e Engenharia Florestal. O NPDEAS
            entende que o desenvolvimento de Ciência e Tecnologia é estratégico
            para o desenvolvimento de um país. A inovação de produtos, processos
            ou modelos de negócio podem catalisar as modificações necessárias
            para a melhoria econômica de uma nação e alavancar o aumento
            sustentável da qualidade de vida da população. As universidades
            compõem o celeiro do desenvolvimento científico e tecnológico e,
            desta forma, são os atores com capacidade de iniciar essa
            transformação.
          </h5>
          <div class="VisitasTexto alignButton">
            <div>
              <v-btn
                large
                rounded
                color="#fcd24a"
                class="black--text"
                href="/visitas"
              >
                Saiba mais
                <v-icon right dark>mdi-rocket</v-icon>
              </v-btn>
            </div>
            <div class="marginleft">
              <v-btn large rounded color="#fcd24a" class="black--text">
                Agende sua visita
                <v-icon right dark>mdi-rocket</v-icon>
              </v-btn>
            </div>
          </div>
        </v-card>
        <v-card v-else width="700px" class="marginCard" color="#fcd24a">
          <v-img
            src="/imagens/visita.JPG"
            class="ImageSize justify-end"
          ></v-img>
        </v-card>
      </v-col>
    </v-row>
  </v-container-fluid>
</template>

<script>
export default {}
</script>

<style scoped>
.margin {
  padding-top: 3%;
}

.paddingText {
  padding-left: 30px;
  padding-right: 30px;
}

.marginCard {
  padding-right: 15px;
}

.ImageSize {
  height: 700px;
  width: 700px;
}

.VisitasTexto {
  padding-left: 10%;
  padding-right: 10%;
  margin-top: 8%;
}

.VisitasTitle {
  color: #fcd24a;
  font-weight: bold;
  text-align: center;
  font-size: 30px;
  font-family: 'Arapey', 'Montserrat';
}

.VisitasText {
  text-align: justify;
  margin-top: 5%;
  font-size: 15px;
  color: white;
}

.alignButton {
  display: flex;
  flex-direction: row;
  align-items: center;
  align-self: flex-end;
  margin-top: 10%;
}

.VisitasColor {
  background-color: #10041c;
}

.marginleft {
  margin-left: 25%;
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
  .ImageSize {
    height: 360px;
    width: 460px;
  }

  .VisitasTexto {
    padding-left: 10%;
    padding-right: 10%;
    margin-top: 5%;
  }

  .marginImage {
    height: 500px;
  }
}
</style>
