<template>
  <v-container fluid class="NavbarGeral">
    <v-container fluid class="navbarSize d-none d-lg-flex">
      <v-toolbar height="110" flat color="white">
        <v-spacer class="d-none d-lg-flex"></v-spacer>
        <v-toolbar-title class="d-none d-lg-flex">
          <router-link to="/" tag="span" style="cursor: pointer;">
            <v-img
              max-width="60"
              max-height="60"
              src="/imagens/Icons/LogoCPT.png"
            />
          </router-link>
        </v-toolbar-title>
        <v-spacer></v-spacer>
        <v-toolbar-items class="d-none d-lg-flex">
          <v-btn
            v-for="(item, i) in items"
            :key="i"
            :to="item.link"
            depressed
            small
            text
            class="navbar-button navCor"
          >
            <p
              v-if="item.title === 'LOGIN'"
              class="navbar-button ButtonContact white--text"
              v-bind="attrs"
              v-on="on"
            >
              {{ item.title }}
            </p>
            <p v-else :class="button" v-bind="attrs" v-on="on">
              {{ item.title }}
            </p>
          </v-btn>
        </v-toolbar-items>
        <v-spacer class="d-md-none d-lg-flex"></v-spacer>
      </v-toolbar>
    </v-container>
    <v-container class="NavbarGeral d-lg-none">
      <div class="NavbarGeralOne">
        <v-app-bar-nav-icon
          class="icon d-lg-none"
          @click.stop="drawer = !drawer"
        ></v-app-bar-nav-icon>
        <v-toolbar-title class="d-lg-none d-md-flex centerImg">
          <router-link to="/" tag="span" style="cursor: pointer;">
            <v-img
              max-width="180"
              max-height="70"
              src="/imagens/Icons/LogoCPT.png"
            />
          </router-link>
        </v-toolbar-title>
      </div>
      <v-navigation-drawer v-model="drawer" absolute temporary>
        <v-list dense>
          <v-list-item v-for="(item, l) in items" :key="l" link>
            <v-list-item-content>
              <v-list-item-title class="navbar-button navCor">{{
                item.title
              }}</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list>
      </v-navigation-drawer>
    </v-container>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      bg: 'transparent',
      button: 'navbar-button navbarButtonColor navCor',
      drawer: false,
      items: [
        {
          title: 'INÍCIO',
          link: '/',
        },
        {
          title: 'QUEM SOMOS',
          link: '/AboutUs',
        },
        {
          title: 'BLOG',
          link: '/blog',
        },
        {
          title: 'EVENTOS',
          link: '/events',
        },
        {
          title: 'EQUIPE',
          link: '/equipe',
        },
        {
          title: 'STARTUPS',
          link: '/startups',
        },
        {
          title: 'CONTATO',
          link: '/contato',
        },
        {
          title: 'LOGIN',
          link: '/login',
        },
      ],
    }
  },

  mounted() {
    window.addEventListener('scroll', this.onScroll)
  },
  beforeDestroy() {
    window.removeEventListener('scroll', this.onScroll)
  },
  methods: {
    onScroll() {
      if (window.scrollY > 100) {
        this.button = 'navbar-button navCor'
        this.logo = '../imagens/logoUp.png'
      } else if (window.scrollY === 0) {
        this.bg = 'transparent'
        this.button = 'navbar-button navbarButtonColor navCor'
        this.logo = '../imagens/logoUpOne.png'
      }
    },
  },
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@600&display=swap');

.icon {
  margin-left: 20px;
  align-self: center;
  margin-right: 20px;
}

.centerImg {
  align-self: center;
}

.navbarSize {
  padding: 0px;
  position: fixed;
  z-index: 1000;
}

.NavbarGeral {
  padding: 0px;
}

.NavbarGeralOne {
  display: flex;
  flex-direction: row;
  height: 100px;
}

.SizeMobile {
  height: 100px;
}

.v-btn:before {
  background-color: transparent;
}

.ButtonContact {
  color: black;
  height: 50px;
  width: 110px;
  background-color: #3fa944;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 30px;
}

.ButtonContact:hover {
  transform: translateX(0px) scale(1.1);
}

.navbar-button {
  text-transform: capitalize;
  font-family: 'Open Sans', sans-serif;
  font-size: 15px;
  margin-right: 15px;
  font-weight: bold;
  margin-bottom: 0px;
}

.navbarButtonColor {
  color: black;
}

.navCor:hover {
  color: #3fa944;
}

.v-btn:not(.v-btn--round).v-size--small {
  padding: 0;
}
</style>
