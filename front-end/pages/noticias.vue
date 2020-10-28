<template>
  <v-app class="NoticiaColor">
    <Inicio titulo="Notícias" imagem="/imagens/Fundos/1876.jpg" />
    <v-container-fluid class="marginNoticias">
      <v-row>
        <v-col cols="12">
          <h1 class="TitleNoticias">Destaques</h1>
        </v-col>
      </v-row>
      <v-row>
        <v-col
          v-for="item in noticiasDestaque"
          :key="item.titulo"
          cols="12"
          md="6"
          sm="6"
          lg="4"
        >
          <Noticia
            :titulo="item.titulo"
            :imagem="item.imagem"
            :texto="item.texto"
          />
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="12">
          <h1 class="TitleNoticias margin">Últimas notícias</h1>
        </v-col>
      </v-row>
      <v-row>
        <v-col
          v-for="item in ultimasnoticias"
          :key="item.titulo"
          cols="12"
          md="6"
          sm="6"
          lg="4"
        >
          <Noticia
            :titulo="item.titulo"
            :imagem="item.imagem"
            :texto="item.texto"
          />
        </v-col>
      </v-row>
      <v-pagination
        v-model="page"
        class="margin"
        color="#230c3d"
        circle
        :length="length"
        :next-icon="nextIcon"
        :prev-icon="prevIcon"
        :page="page"
        :total-visible="totalVisible"
      ></v-pagination>
    </v-container-fluid>
    <Footer />
  </v-app>
</template>

<script>
import Inicio from '../components/Inicio'
import Noticia from '../components/SectionsNoticias/Noticia'
import Footer from '../components/Footer'

export default {
  components: {
    Footer,
    Inicio,
    Noticia,
  },
  data() {
    return {
      length: 5,
      nextIcons: 'mdi-chevron-right',
      prevIcons: 'mdi-chevron-left',
      page: 1,
      totalVisible: 5,
      noticiasDestaque: [
        {
          titulo:
            'Engenharia Elétrica marca presença no I Workshop Internacional de Tecnologias Assistivas',
          imagem: '/imagens/HomeFoto.JPG',
          texto:
            'Alunos do Departamento de Engenharia Elétrica apresentaram dois trabalhos no "I Workshop Internacional de Tecnologias Assistivas" realizado pelo Governo do Estado do Paraná ...',
        },
        {
          titulo: 'Alunos do Ciência para Todos participam do INNOVATION DAY',
          imagem: '/imagens/inovacao.jpg',
          texto:
            'Alunos do Departamento de Engenharia Elétrica apresentaram dois trabalhos no "I Workshop Internacional de Tecnologias Assistivas" realizado pelo Governo do Estado do Paraná ...',
        },
        {
          titulo:
            'Alunos do projeto Ciência para Todos entre os 100 melhores projetos de Startup do Paraná',
          imagem: '/imagens/seLiga.jpg',
          texto:
            'Alunos do Departamento de Engenharia Elétrica apresentaram dois trabalhos no "I Workshop Internacional de Tecnologias Assistivas" realizado pelo Governo do Estado do Paraná ...',
        },
      ],
      ultimasnoticias: [
        {
          titulo:
            'Engenharia Elétrica marca presença no I Workshop Internacional de Tecnologias Assistivas',
          imagem: '/imagens/HomeFoto.JPG',
          texto:
            'Alunos do Departamento de Engenharia Elétrica apresentaram dois trabalhos no "I Workshop Internacional de Tecnologias Assistivas" realizado pelo Governo do Estado do Paraná ...',
        },
        {
          titulo: 'Alunos do Ciência para Todos participam do INNOVATION DAY',
          imagem: '/imagens/inovacao.jpg',
          texto:
            'Alunos do Departamento de Engenharia Elétrica apresentaram dois trabalhos no "I Workshop Internacional de Tecnologias Assistivas" realizado pelo Governo do Estado do Paraná ...',
        },
        {
          titulo:
            'Alunos do projeto Ciência para Todos entre os 100 melhores projetos de Startup do Paraná',
          imagem: '/imagens/seLiga.jpg',
          texto:
            'Alunos do Departamento de Engenharia Elétrica apresentaram dois trabalhos no "I Workshop Internacional de Tecnologias Assistivas" realizado pelo Governo do Estado do Paraná ...',
        },
        {
          titulo:
            'Engenharia Elétrica marca presença no I Workshop Internacional de Tecnologias Assistivas',
          imagem: '/imagens/HomeFoto.JPG',
          texto:
            'Alunos do Departamento de Engenharia Elétrica apresentaram dois trabalhos no "I Workshop Internacional de Tecnologias Assistivas" realizado pelo Governo do Estado do Paraná ...',
        },
        {
          titulo: 'Alunos do Ciência para Todos participam do INNOVATION DAY',
          imagem: '/imagens/inovacao.jpg',
          texto:
            'Alunos do Departamento de Engenharia Elétrica apresentaram dois trabalhos no "I Workshop Internacional de Tecnologias Assistivas" realizado pelo Governo do Estado do Paraná ...',
        },
        {
          titulo:
            'Alunos do projeto Ciência para Todos entre os 100 melhores projetos de Startup do Paraná',
          imagem: '/imagens/seLiga.jpg',
          texto:
            'Alunos do Departamento de Engenharia Elétrica apresentaram dois trabalhos no "I Workshop Internacional de Tecnologias Assistivas" realizado pelo Governo do Estado do Paraná ...',
        },
      ],
    }
  },
  methods: {},
}
</script>

<style scoped>
.marginNoticias {
  margin-left: 15%;
  margin-right: 15%;
  margin-top: 5%;
  margin-bottom: 5%;
}

.margin {
  margin-top: 5%;
  margin-left: 0;
}

.NoticiaColor {
  background-color: #10041c;
}

.TitleNoticias {
  color: #fcd24a;
}
</style>
