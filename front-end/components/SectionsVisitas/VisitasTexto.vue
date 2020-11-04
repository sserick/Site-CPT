<template>
  <v-container-fluid class="SobreColor">
    <v-row justify="center">
      <v-col cols="8" class="SobreTexto">
        <h2 class="fontTitle">Agende uma visita conosco!!!</h2>
      </v-col>
      <v-col cols="8" class="SobreTexto">
        <h3>O PROJETO</h3>
      </v-col>
      <v-col cols="8" class="SobreTexto">
        O Projeto de Extensão Ciência para Todos da Universidade Federal do
        Paraná tem por objetivo geral desenvolver e aplicar ferramentas de
        gestão do processo de inovação através da aplicação de plataformas de
        transferência de tecnologia e treinamento de alunos de graduação em
        atividades extensionistas com foco na interação com professores e alunos
        de escolas do ensino fundamental, médio e profissional. Para isso o
        projeto conta com a infraestrutura do NPDEAS, Núcleo de Pesquisa e
        Desenvolvimento de Energia Autossustentável, que desde 2008 trabalho no
        desenvolvimento de tecnologias em escala de engenharia na área de
        energias renováveis, meio ambiente e biotecnologia.
      </v-col>
      <v-col cols="8" class="SobreTexto">
        <h3>COMO AGENDAR AS VISITAS?</h3>
      </v-col>
      <v-col cols="8" class="SobreTexto">
        Os professores interessados em realizar uma visita ao NPDEAS com seus
        alunos devem preencher um cadastro disponível neste endereço: Formulário
        de Agendamento. As visitas devem ser acompanhadas pelo professor
        representante da escola ou colégio e estão limitadas ao número máximo de
        35 alunos. Não existe qualquer custo para essa visita. Os agendamentos
        são realizados em períodos que não afetem o funcionamento do NPDEAS.
      </v-col>
      <v-col cols="8" class="SobreTexto">
        <h3>COMO SÃO AS VISITAS?</h3>
      </v-col>
      <v-col cols="8" class="SobreTexto">
        As visitas tem duração de 2 horas e incluem um tour por toda a
        infraestrutura do NPDEAS incluindo:
      </v-col>
      <v-col cols="8" class="SobreTexto">
        <ul>
          <li>Laboratório de Biotecnologia</li>
          <li>Laboratório de Cultivo de Microalgas</li>
          <li>Unidade de Produção de Biodiesel</li>
          <li>Unidade de Explosão a Vapor</li>
          <li>Laboratório de Química Pesada</li>
          <li>Unidade de Fotobiorreatores</li>
          <li>Unidade de Tratamento de Resíduos Sólidos Urbanos</li>
          <li>Unidade de Operações Unitárias Avançadas</li>
          <li>Unidade de Tratamento de Emissões Atmosféricas</li>
          <li>Unidade de Biodigestão de Resíduos Orgânicos</li>
        </ul>
      </v-col>
      <v-col cols="8" class="SobreTexto">
        A visita é acompanhada pelo coordenador do projeto e por alunos de
        graduação pertencentes ao projeto. Os alunos visitantes vão receber
        orientações a respeito de todas as pesquisas realizadas em cada setor do
        NPDEAS.
      </v-col>
      <v-col cols="8">
        <v-row justify="center">
          <v-card width="700px" class="marginCard" color="#fcd24a">
            <v-img
              src="/imagens/visita.JPG"
              class="ImageSize justify-end"
            ></v-img>
          </v-card>
        </v-row>
      </v-col>
      <v-col cols="8" class="marginBottom">
        <v-row justify="center">
          <v-btn
            href="/visitas"
            large
            rounded
            color="#fcd24a"
            class="black--text button"
          >
            Agende sua visita
            <v-icon right dark>mdi-rocket</v-icon>
          </v-btn>
        </v-row>
      </v-col>
    </v-row>
  </v-container-fluid>
</template>

<script>
export default {}
</script>

<style scoped>
.ImageSize {
  height: 500px;
  width: 700px;
}

.SobreColor {
  background-color: #10041c;
  padding-top: 5%;
  padding-bottom: 5%;
}

.fontTitle {
  color: #fcd24a;
}

.marginCard {
  padding-left: 15px;
  padding-right: 15px;
}

.SobreTexto {
  font-size: 18px;
  text-align: justify;
}

.marginBottom {
  margin-top: 3%;
}
</style>
