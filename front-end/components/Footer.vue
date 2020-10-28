<template>
  <v-footer class="py-2" color="#230c3d" padless>
    <v-row justify="center" no-gutters>
      <v-btn
        v-for="link in links"
        :key="link.link"
        :href="link.link"
        color="white"
        text
        rounded
        class="my-2"
      >
        {{ link.nome }}
      </v-btn>
      <v-card-text class="text-center">
        <v-btn
          v-for="icon in icons"
          :key="icon.icon"
          :href="icon.link"
          class="mx-4 white--text"
          icon
        >
          <v-icon size="24px">{{ icon.icon }}</v-icon>
        </v-btn>
      </v-card-text>
      <v-col class="MVVColor py-2 text-center white--text" cols="12">
        © Copyright Ciência para Todos. All Rights Reserved
      </v-col>
      <v-col class="MVVColor py-2 text-center white--text" cols="12">
        Desenvolvido por
        <a class="links" href="" target="_blank">Erick Santos</a>
        e
        <a class="links" href="" target="_blank">Mirele Miranda</a>
      </v-col>
    </v-row>
  </v-footer>
</template>

<script>
export default {
  data: () => ({
    variant: 'absolute',
    links: [
      { nome: 'Início', link: '/' },
      { nome: 'Notícias', link: '/noticias' },
      { nome: 'Eventos', link: '/eventos' },
      { nome: 'Equipe', link: '/equipe' },
      { nome: 'Startups', link: '/startups' },
      { nome: 'Contato', link: '/contato' },
      { nome: 'Sobre nós', link: '/SobreNos' },
      { nome: 'Startup Expirience', link: '/startupeExpirence' },
      { nome: 'Visitas', link: '/visitas' },
    ],
    icons: [
      { icon: 'mdi-facebook', link: '' },
      { icon: 'mdi-twitter', link: '' },
      { icon: 'mdi-linkedin', link: '' },
      { icon: 'mdi-instagram', link: '' },
      { icon: 'mdi-blogger', link: '' },
      { icon: 'mdi-youtube', link: '' },
    ],
  }),
  computed: {
    localAttrs() {
      const attrs = {}
      attrs[this.variant] = true
      return attrs
    },
  },
}
</script>

<style scoped>
.itensNavFooter a:hover {
  color: #50116e;
}

.img {
  width: 70px;
  height: 70px;
}

.imagem {
  align-items: flex-end;
}

a {
  text-decoration: none;
  color: white;
}

.logo {
  height: 120px;
  width: 120px;
  align-self: center;
}

.links {
  font-family: 'Arapey', 'Montserrat';
  font-weight: bold;
}

.MVVColor {
  background-color: #10041c;
}
</style>
