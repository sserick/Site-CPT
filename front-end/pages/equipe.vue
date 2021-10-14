<template>
  <v-app class="EquipeColor">
    <initial />
    <v-container-fluid class="marginEquipe">
      <v-row justify="center">
        <v-col cols="8">
          <equipe :messages="intituicoes" title="Instituições" />
        </v-col>
        <v-col cols="8">
          <equipe :messages="parcerias" title="Parcerias" />
        </v-col>
        <v-col cols="8">
          <equipe :messages="professores" title="Professores" />
        </v-col>
        <v-col cols="8">
          <equipe :messages="alunos" title="Alunos" />
        </v-col>
        <v-col cols="8">
          <equipe :messages="exalunos" title="Ex-Alunos" />
        </v-col>
      </v-row>
    </v-container-fluid>
  </v-app>
</template>

<script>
import initial from '../components/SectionsHome/Inicio.vue'
import equipe from '../components/SectionsEquipe/Equipe.vue'

export default {
  components: {
    initial,
    equipe,
  },
  data() {
    return {
      intituicoes: [
        {
          avatar: 'https://avatars0.githubusercontent.com/u/9064066?v=4&s=460',
          name: 'UFPR',
          title: 'Universidade Federal do Paraná',
          text: 'Thank you for joining our community...',
          facebook: 'https://www.facebook.com/',
          instagram: '',
          linkedln: '',
        },
        {
          avatar: 'https://avatars0.githubusercontent.com/u/9064066?v=4&s=460',
          name: 'CPT',
          title: 'Ciência para Todos',
          text: 'Thank you for joining our community...',
          facebook: 'https://www.facebook.com/',
          instagram: '',
          linkedln: '',
        },
        {
          avatar: 'https://avatars0.githubusercontent.com/u/9064066?v=4&s=460',
          name: 'NPDEAS',
          title:
            'Núcleo de Pesquisa e Desenvolvimento de Energia Autossustentável',
          text: 'Thank you for joining our community...',
          facebook: 'https://www.facebook.com/',
          instagram: '',
          linkedln: '',
        },
      ],
      parcerias: [
        {
          name: 'Parcerias 1',
          title: 'Universidade Federal do Paraná',
          image: '/imagens/Icons/institui.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
        {
          name: 'Parcerias 2',
          title: 'Universidade Federal do Paraná',
          image: '/imagens/Icons/institui.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
        {
          name: 'Parcerias 3',
          title: 'Universidade Federal do Paraná',
          image: '/imagens/Icons/institui.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
      ],
      professores: [
        {
          name: 'Professores 1',
          title: 'Universidade Federal do Paraná',
          image: '/imagens/homem.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
        {
          name: 'Professores 2',
          title: 'Universidade Federal do Paraná',
          image: '/imagens/homem.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
        {
          name: 'Professores 3',
          title: 'Universidade Federal do Paraná',
          image: '/imagens/homem.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
      ],
      alunos: [
        {
          name: 'Alunos 1',
          title: 'Universidade Federal do Paraná',
          image: '/imagens/Icons/aluno.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
        {
          name: 'Alunos 2',
          title: 'Universidade Federal do Paraná',
          image: '/imagens/Icons/aluno.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
        {
          name: 'Alunos 3',
          title: 'Universidade Federal do Paraná',
          image: '/imagens/Icons/aluno.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
      ],
      exalunos: [
        {
          name: 'Ex aluno 1',
          title: 'Universidade Federal do Paraná',
          image: '/imagens/Icons/aluno.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
        {
          name: 'Ex aluno 2',
          title: 'Universidade Federal do Paraná',
          image: '/imagens/Icons/aluno.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
        {
          name: 'Ex aluno 3',
          title: 'Universidade Federal do Paraná',
          image: '/imagens/Icons/aluno.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
      ],
    }
  },
  methods: {},
}
</script>

<style scoped>
.marginEquipe {
  margin-top: 5%;
  margin-bottom: 5%;
}

.EquipeColor {
  background-color: RGBA(63, 169, 68, 0.05);
}
</style>
