<template>
  <v-app class="EquipeColor">
    <Inicio titulo="Equipe" />
    <v-container-fluid class="marginEquipe">
      <v-row justify="center">
        <v-col cols="8">
          <Equipe :messages="intituicoes" title="Instituições" />
        </v-col>
        <v-col cols="8">
          <Equipe :messages="intituicoes" title="Parcerias" />
        </v-col>
        <v-col cols="8">
          <Equipe :messages="intituicoes" title="Professores" />
        </v-col>
        <v-col cols="8">
          <Equipe :messages="intituicoes" title="Alunos" />
        </v-col>
        <v-col cols="8">
          <Equipe :messages="intituicoes" title="Ex-Alunos" />
        </v-col>
      </v-row>
    </v-container-fluid>
    <Footer />
  </v-app>
</template>

<script>
import Inicio from '../components/Inicio'
import Equipe from '../components/SectionsEquipe/Equipe'
import Footer from '../components/Footer'

export default {
  components: {
    Footer,
    Inicio,
    Equipe,
  },
  data() {
    return {
      intituicoes: [
        {
          avatar: 'https://avatars0.githubusercontent.com/u/9064066?v=4&s=460',
          name: 'Erick Santos',
          title: 'Welcome to Vuetify!',
          text: 'Thank you for joining our community...',
          facebook: 'https://www.facebook.com/',
          instagram: '',
          linkedln: '',
        },
        {
          avatar: 'https://avatars0.githubusercontent.com/u/9064066?v=4&s=460',
          name: 'Mirele Miranda',
          title: 'Welcome to Vuetify!',
          text: 'Thank you for joining our community...',
          facebook: 'https://www.facebook.com/',
          instagram: '',
          linkedln: '',
        },
        {
          avatar: 'https://avatars0.githubusercontent.com/u/9064066?v=4&s=460',
          name: 'Beatriz Furlan',
          title: 'Welcome to Vuetify!',
          text: 'Thank you for joining our community...',
          facebook: 'https://www.facebook.com/',
          instagram: '',
          linkedln: '',
        },
      ],
      parcerias: [
        {
          name: 'Parcerias 1',
          image: '/imagens/Icons/institui.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
        {
          name: 'Parcerias 2',
          image: '/imagens/Icons/institui.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
        {
          name: 'Parcerias 3',
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
          image: '/imagens/homem.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
        {
          name: 'Professores 2',
          image: '/imagens/homem.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
        {
          name: 'Professores 3',
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
          image: '/imagens/Icons/aluno.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
        {
          name: 'Alunos 2',
          image: '/imagens/Icons/aluno.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
        {
          name: 'Alunos 3',
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
          image: '/imagens/Icons/aluno.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
        {
          name: 'Ex aluno 2',
          image: '/imagens/Icons/aluno.png',
          face: 'https://www.google.com/',
          insta: 'https://www.youtube.com/',
          twitter: 'https://www.google.com.br/maps',
          linkdln: 'https://calendar.google.com/calendar',
        },
        {
          name: 'Ex aluno 3',
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
  background-color: #10041c;
}
</style>
