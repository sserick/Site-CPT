<template>
  <v-app>
    <initial />
    <blog :blog="highlights" title="Destaques" />
    <blog :blog="blog" title="Últimas postagens" />
    <v-row justify="center" align="center" class="Pagination">
      <v-col cols="10" md="10" lg="5" xl="5">
        <v-row justify="center" align="center">
          <v-pagination
            v-model="page"
            color="#3fa944"
            :length="6"
            circle
          ></v-pagination>
        </v-row>
      </v-col>
    </v-row>
  </v-app>
</template>

<script>
import initial from '../components/SectionsHome/Inicio.vue'
import blog from '../components/SectionBlog/Blog.vue'

export default {
  components: {
    initial,
    blog,
  },
  data() {
    return {
      page: 1,
      highlights: [
        {
          imgFundo: '/imagens/seLiga.jpg',
          imgPerson: '/imagens/homem.png',
          title: 'ESTUDO DE VIABILIDADE',
          date: '24 de Julho de 2021',
          link: '/',
          text:
            'O empreendedorismo esta em alta, você sonha em ter a sua empresa, mas não sabe dos riscos? Não arrisque seu dinheiro, invista com segurança, muitos empreendedores tem seus sonhos aruinados por [...]',
        },
        {
          imgFundo: '/imagens/seLiga.jpg',
          imgPerson: '/imagens/homem.png',
          title: 'ESTUDO DE VIABILIDADE',
          date: '24 de Julho de 2021',
          link: '/',
          text:
            'O empreendedorismo esta em alta, você sonha em ter a sua empresa, mas não sabe dos riscos? Não arrisque seu dinheiro, invista com segurança, muitos empreendedores tem seus sonhos aruinados por [...]',
        },
        {
          imgFundo: '/imagens/seLiga.jpg',
          imgPerson: '/imagens/homem.png',
          title: 'ESTUDO DE VIABILIDADE',
          date: '24 de Julho de 2021',
          link: '/',
          text:
            'O empreendedorismo esta em alta, você sonha em ter a sua empresa, mas não sabe dos riscos? Não arrisque seu dinheiro, invista com segurança, muitos empreendedores tem seus sonhos aruinados por [...]',
        },
      ],
      blog: [
        {
          imgFundo: '/imagens/seLiga.jpg',
          imgPerson: '/imagens/homem.png',
          title: 'ESTUDO DE VIABILIDADE',
          date: '24 de Julho de 2021',
          link: '/',
          text:
            'O empreendedorismo esta em alta, você sonha em ter a sua empresa, mas não sabe dos riscos? Não arrisque seu dinheiro, invista com segurança, muitos empreendedores tem seus sonhos aruinados por [...]',
        },
        {
          imgFundo: '/imagens/seLiga.jpg',
          imgPerson: '/imagens/homem.png',
          title: 'ESTUDO DE VIABILIDADE',
          date: '24 de Julho de 2021',
          link: '/',
          text:
            'O empreendedorismo esta em alta, você sonha em ter a sua empresa, mas não sabe dos riscos? Não arrisque seu dinheiro, invista com segurança, muitos empreendedores tem seus sonhos aruinados por [...]',
        },
        {
          imgFundo: '/imagens/seLiga.jpg',
          imgPerson: '/imagens/homem.png',
          title: 'ESTUDO DE VIABILIDADE',
          date: '24 de Julho de 2021',
          link: '/',
          text:
            'O empreendedorismo esta em alta, você sonha em ter a sua empresa, mas não sabe dos riscos? Não arrisque seu dinheiro, invista com segurança, muitos empreendedores tem seus sonhos aruinados por [...]',
        },
        {
          imgFundo: '/imagens/seLiga.jpg',
          imgPerson: '/imagens/homem.png',
          title: 'ESTUDO DE VIABILIDADE',
          date: '24 de Julho de 2021',
          link: '/',
          text:
            'O empreendedorismo esta em alta, você sonha em ter a sua empresa, mas não sabe dos riscos? Não arrisque seu dinheiro, invista com segurança, muitos empreendedores tem seus sonhos aruinados por [...]',
        },
        {
          imgFundo: '/imagens/seLiga.jpg',
          imgPerson: '/imagens/homem.png',
          title: 'ESTUDO DE VIABILIDADE',
          date: '24 de Julho de 2021',
          link: '/',
          text:
            'O empreendedorismo esta em alta, você sonha em ter a sua empresa, mas não sabe dos riscos? Não arrisque seu dinheiro, invista com segurança, muitos empreendedores tem seus sonhos aruinados por [...]',
        },
        {
          imgFundo: '/imagens/seLiga.jpg',
          imgPerson: '/imagens/homem.png',
          title: 'ESTUDO DE VIABILIDADE',
          date: '24 de Julho de 2021',
          link: '/',
          text:
            'O empreendedorismo esta em alta, você sonha em ter a sua empresa, mas não sabe dos riscos? Não arrisque seu dinheiro, invista com segurança, muitos empreendedores tem seus sonhos aruinados por [...]',
        },
      ],
    }
  },
  methods: {},
}
</script>

<style scoped>
.Pagination {
  background-color: RGBA(63, 169, 68, 0.05);
  padding-bottom: 3%;
}
</style>
