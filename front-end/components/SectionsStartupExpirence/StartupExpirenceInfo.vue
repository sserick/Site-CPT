<template>
  <v-container fluid class="StartupExpirenceColor">
    <v-row justify="center" align="center">
      <v-col cols="8" class="StartupExpirenceTexto">
        <h2 class="fontTitle">Começo de uma nova jornada</h2>
      </v-col>
      <v-col cols="8" class="StartupExpirenceTexto">
        <p>
          Desde a fundação do NPDEAS os coordenadoras realizam atividades como
          visitas dirigidas aos laboratórios do grupo de pesquisa. Várias
          escolas e universidades do Brasil e do Mundo passaram pelos
          laboratórios e conheceram as pesquisas realizadas na UFPR com foco em
          Energia Renovável, Biotecnologia e Meio Ambiente.
        </p>
      </v-col>
      <v-col cols="8" class="StartupExpirenceTexto">
        <p>
          Agora, a partir de Agosto de 2016, o NPDEAS conta com o Projeto de
          Extensão Universitária destinado divulgação da Ciência, Tecnologia e
          Inovação para a Sociedade. Trata-se do CIÊNCIA PARA TODOS que tem como
          público alvo alunos, funcionários e professores de escolas do ensino
          fundamental, médio e profissional.
        </p>
      </v-col>
      <v-col cols="8" class="StartupExpirenceTexto">
        <p>
          O projeto contará com o envolvimento de professores e alunos da UFPR
          responsáveis pela realização das atividades ao público alvo.
        </p>
      </v-col>
      <v-col cols="8" class="StartupExpirenceTexto">
        <p>
          Neste projeto haverá o envolvimento dos alunos da graduação que vão
          receber capacitação para realizar as atividades propostas de
          divulgação da Ciência para a comunidade.
        </p>
      </v-col>
      <v-col cols="8" class="StartupExpirenceTexto">
        <p>
          Assim como o NPDEAS, este projeto de extensão é essencialmente
          interdisciplinar e vai contar inicialmente com alunos de graduação de
          diversas áreas da Universidade como, por exemplo, os cursos de
          Biotecnologia, Biologia, Engenharia Química, Engenharia Elétrica,
          Engenharia Mecânica e Engenharia Florestal.
        </p>
      </v-col>
      <v-col cols="8" class="StartupExpirenceTexto">
        <p>
          O NPDEAS entende que o desenvolvimento de Ciência e Tecnologia é
          estratégico para o desenvolvimento de um país. A inovação de produtos,
          processos ou modelos de negócio podem catalisar as modificações
          necessárias para a melhoria econômica de uma nação e alavancar o
          aumento sustentável da qualidade de vida da população. As
          universidades compõem o celeiro do desenvolvimento científico e
          tecnológico e, desta forma, são os atores com capacidade de iniciar
          essa transformação.
        </p>
      </v-col>
      <v-col cols="8">
        <v-row justify="center" align="center">
          <v-card width="700px" class="marginCard" color="#fcd24a">
            <v-row justify="center" align="center">
              <v-img
                src="/imagens/Icons/startup.png"
                class="ImageSize justify-end"
                contain
              ></v-img>
            </v-row>
          </v-card>
        </v-row>
      </v-col>
      <v-col cols="8" class="StartupExpirenceTexto">
        <p>
          A nossa experiência nos mostra que se faz necessário uma articulação
          entre a universidade, a sociedade e o setor produtivo para:
        </p>
      </v-col>
      <v-col cols="8" class="StartupExpirenceTexto">
        <p>
          O objetivo principal do projeto consiste em:
        </p>
      </v-col>
      <v-col cols="8" class="StartupExpirenceTexto">
        <p>
          "Desenvolver e aplicar ferramentas de gestão do processo de inovação
          através da aplicação de plataformas de transferência de tecnologia e
          treinamento de alunos de graduação em atividades de extensão com foco
          em Professores e Alunos de escolas do ensino fundamental, médio e
          profissional baseado no trabalho do NPDEAS, grupo de pesquisa
          interdisciplinar da UFPR em energia autossustentável, meio ambiente e
          biotecnologia, através de visitas dirigidas e canais de comunicação de
          via dupla com a sociedade".
        </p>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {}
</script>

<style scoped>
.ImageSize {
  height: 500px;
  width: 700px;
}

.StartupExpirenceColor {
  background-color: RGBA(63, 169, 68, 0.05);
  padding-top: 5%;
  padding-bottom: 5%;
}

.fontTitle {
  color: #3fa944;
}

.marginCard {
  padding-left: 15px;
  padding-right: 15px;
}

.alignmargin {
  padding-top: 2%;
  padding-bottom: 2%;
}

.StartupExpirenceTexto {
  font-size: 18px;
  text-align: justify;
}
</style>
