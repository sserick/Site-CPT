<template>
  <v-app>
    <nuxt />
    <div>
      <v-app-bar color="#10041c" height="80px" flat fixed>
        <v-spacer></v-spacer>

        <div class="logo">
          <v-img
            alt="Logo do Ciência para Todos"
            src="/imagens/Icons/LogoCPT.png"
            aspect-ratio="1"
            @click="$router.push('/')"
          ></v-img>
        </div>
        <div class="NameCPT">
          <v-img
            contain
            alt="Ciência para Todos"
            src="/imagens/Icons/Imagem6.png"
            aspect-ratio="1"
            @click="$router.push('/')"
          ></v-img>
        </div>

        <v-spacer></v-spacer>
        <v-spacer></v-spacer>
        <v-app-bar-nav-icon
          id="Navigation"
          color="#fff"
          class="hidden-lg-and-up"
          @click="drawer = !drawer"
        >
        </v-app-bar-nav-icon>

        <v-btn
          depressed
          large
          color="#10041c"
          class="hidden-md-and-down Item text-capitalize"
          href="/"
          ><a>Inicío</a></v-btn
        >
        <v-btn
          depressed
          large
          color="#10041c"
          class="hidden-md-and-down Item text-capitalize"
          href="/noticias"
          ><a href="/noticias">Notícias</a></v-btn
        >

        <v-btn
          depressed
          large
          color="#10041c"
          class="hidden-md-and-down Item text-capitalize"
          href="/eventos"
          ><a href="/eventos">Eventos</a></v-btn
        >

        <v-btn
          depressed
          large
          color="#10041c"
          class="hidden-md-and-down Item text-capitalize"
          href="/equipe"
          ><a href="/equipe">Equipe</a></v-btn
        >

        <div depressed class="hidden-md-and-down boto" color="#10041c">
          <v-menu offset-y>
            <template v-slot:activator="{ on }">
              <v-btn
                color="#10041c"
                depressed
                large
                class="hidden-md-and-down Item text-capitalize botoes"
                v-on="on"
              >
                <a class="Item">Startup's</a
                ><v-icon color="#fff">mdi-chevron-down</v-icon>
              </v-btn>
            </template>
            <v-list class="listin" light>
              <v-list-item v-for="drop in drops" :key="drop.title">
                <a class="droplista">
                  <v-list-item-title class="link"
                    ><a href="/startupOne">{{
                      drop.title
                    }}</a></v-list-item-title
                  >
                </a>
              </v-list-item>
            </v-list>
          </v-menu>
        </div>

        <v-btn
          large
          depressed
          color="#10041c"
          class="hidden-md-and-down Item text-capitalize"
          href="/contato"
          ><a href="/contato">Contato</a></v-btn
        >

        <v-btn
          large
          depressed
          color="#fcd24a"
          class="hidden-md-and-down Item text-capitalize"
          href="/dashboard"
          ><a href="/contato" class="black--text">Login</a></v-btn
        >

        <v-spacer></v-spacer>
      </v-app-bar>
      <v-navigation-drawer v-model="drawer" color="#10041c" app>
        <v-list dense>
          <v-list-item-group color="white">
            <v-list-item>
              <v-list-item-content>
                <v-list-item-title class="ItemDrawer"
                  ><a href="/">Inicío</a></v-list-item-title
                >
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                <v-list-item-title class="ItemDrawer"
                  ><a href="/noticias">Notícias</a></v-list-item-title
                >
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                <v-list-item-title class="ItemDrawer"
                  ><a href="/eventos">Eventos</a></v-list-item-title
                >
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                <v-list-item-title class="ItemDrawer"
                  ><a href="/equipe">Equipe</a></v-list-item-title
                >
              </v-list-item-content>
            </v-list-item>
            <v-list-group no-action>
              <template v-slot:activator>
                <v-list-item style="padding: 0px;">
                  <v-list-item-content>
                    <v-list-item-title class="ItemDrawer"
                      ><a href="/startups">Startup's</a></v-list-item-title
                    >
                  </v-list-item-content>
                </v-list-item>
              </template>

              <v-list-item v-for="drop in drops" :key="drop.title" link>
                <v-list-item-content>
                  <v-list-item-title class="nav-icons ItemDrawer"
                    ><a href="/startupOne">{{
                      drop.title
                    }}</a></v-list-item-title
                  >
                </v-list-item-content>
              </v-list-item>
            </v-list-group>
            <v-list-item>
              <v-list-item-content>
                <v-list-item-title class="ItemDrawer"
                  ><a href="/contato">Contato</a></v-list-item-title
                >
              </v-list-item-content>
            </v-list-item>
          </v-list-item-group>
        </v-list>
      </v-navigation-drawer>
    </div>
  </v-app>
</template>

<script>
export default {
  components: {},
  data: () => {
    return {
      drawer: false,
      drops: [
        {
          title: 'Startup 1',
          href: '/startupOne',
        },
        {
          title: 'Startup 2',
          href: '',
        },
        {
          title: 'Startup 3',
          href: '',
        },
        {
          title: 'Startup 4',
          href: '',
        },
        {
          title: 'Startup 5',
          href: '',
        },
      ],
    }
  },
}
</script>

<style scoped>
#Title {
  font-size: 20px;
  font-family: 'Arapey', 'Montserrat';
}

#Title a {
  text-decoration: none;
  color: white;
}

.col-xs-12 {
  display: none;
}

.logo {
  height: 50px;
  width: 50px;
  align-self: center;
  margin-right: 10px;
}

.NameCPT {
  height: 150px;
  width: 150px;
  align-self: center;
}

.Textlogo {
  align-self: center;
  margin-top: 10px;
  color: #fdd44d;
}

#Navigation {
  font-size: 2rem;
  cursor: pointer;
}

.Item {
  font-size: 15px;
  font-family: 'Arapey', 'Montserrat';
}

.boto {
  padding: 0;
  margin: 0;
  border-radius: 0%;
}

.botoes {
  font-size: 12px;
  font-family: 'Open Sans', sans-serif;
  border-radius: 0%;
}

.Item a {
  text-decoration: none;
  color: white;
}

.ItemDrawer {
  color: #b02e92;
  font-weight: 500;
  font-family: 'Open Sans', sans-serif;
}

.ItemDrawer a {
  color: #b02e92;
  text-decoration: none;
}

#listin {
  color: #fff;
}

.droplista {
  color: #10041c;
}

.droplista:hover {
  color: #b02e92;
}

.boto {
  background-color: #fff;
}

.link a {
  color: #b02e92;
  text-decoration: none;
}

.nav-icons {
  display: block;
  position: relative;
  color: #d2ece9;
  padding: 0px 15px;
  transition: 0.3s;
  font-size: 14px;
  font-family: 'Open Sans', sans-serif;
}
</style>
