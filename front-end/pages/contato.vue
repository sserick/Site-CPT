<template>
  <v-app>
    <Inicio titulo="Contato" />
    <v-container-fluid>
      <div class="ContatoColor">
        <v-row justify="center">
          <v-col cols="4">
            <h1 class="titleContact">Contato</h1>
            <p class="textContact">
              It is a long established fact that a reader will be distracted by
              the readable content of a page when looking at its layout. The
              point of using Lorem Ipsum is that it has a more-or-less normal
              distribution of letters, as opposed to using 'Content here,
              content here', making it look like readable English. Many desktop
              publishing packages and web page editors now use Lorem Ipsum as
              their default model text, and a search for 'lorem ipsum' will
              uncover many web sites still in their infancy. Various versions
              have evolved over the years, sometimes by accident, sometimes on
              purpose (injected humour and the like). Their default model text,
              componentsIconsand a search for 'lorem ipsum' will uncover many
              web sites still in their infancy. Various versions have evolved
              over the years, sometimes by accident, sometimes on purpose
              (injected humour and the like). Their default model text, and a
              search for 'lorem ipsum' will uncover many web sites still in
              their infancy. Various versions have evolved over the years,
              sometimes by accident, sometimes on purpose (injected humour and
              the like). Their default model text, and a search for 'lorem
              ipsum' will uncover many web sites still in their infancy. Various
              versions have evolved over the years, sometimes by accident,
              sometimes on purpose (injected humour and the like).
            </p>
          </v-col>
          <v-col cols="3" align-self="center" class="contatoConteu">
            <v-row align="center" class="componentsIcons">
              <v-icon x-large color="yellow" class="icons">mdi-email</v-icon>
              <h4>andrebmariano@ufpr.br</h4>
            </v-row>
            <v-row align="center" class="componentsIcons">
              <v-icon x-large color="yellow" class="icons">mdi-phone</v-icon>
              <h4>+55 (41) 3361-3229 (DEP. ENGENHARIA ELÉTRICA - UFPR)</h4>
            </v-row>
            <v-row align="center" class="componentsIcons">
              <v-icon x-large color="yellow" class="icons">mdi-phone</v-icon>
              <h4>+55 (41) 3208-6302 (NPDEAS - UFPR)</h4>
            </v-row>
            <v-row align="center" class="componentsIcons">
              <v-icon x-large color="yellow" class="icons">mdi-phone</v-icon>
              <h4>+55 (41) 3361-3432 (NPDEAS - UFPR)</h4>
            </v-row>
            <v-row align="center">
              <v-icon x-large color="yellow" class="icons">mdi-map</v-icon>
              <h4>
                Francisco H dos Santos, S/N Centro Politécnico, Setor de
                <p>
                  Tecnologia - Jardim das Américas, Curitiba - PR
                </p>
              </h4>
            </v-row>
          </v-col>
        </v-row>
      </div>
      <div class="tamDiv">
        <iframe
          scrolling="no"
          marginheight="0"
          marginwidth="0"
          src="https://maps.google.com/maps?width=100%&amp;height=600&amp;hl=en&amp;q=Av Ataulfo de Paiva 31, Leblon - RIo de Janeiro - RJ +(ProBotox)&amp;t=&amp;z=17&amp;ie=UTF8&amp;iwloc=B&amp;output=embed"
          width="100%"
          height="100%"
          frameborder="0"
        ></iframe>
      </div>
    </v-container-fluid>
    <Footer />
  </v-app>
</template>

<script>
import Footer from '../components/Footer'
import Inicio from '../components/Inicio'

export default {
  components: {
    Footer,
    Inicio
  },
  methods: {}
}
</script>

<style scoped>
.tamDiv {
  height: 400px;
}

.imageSize {
  height: 100%;
  width: 100%;
}

.textContact {
  text-align: justify;
}

.titleContact {
  padding-bottom: 3%;
  color: #fcd24a;
}

.icons {
  margin-right: 15px;
}

.componentsIcons {
  margin-bottom: 7%;
}

.contatoConteu {
  padding-top: 2%;
  margin-left: 3%;
}

.ContatoColor {
  background-color: #10041c;
  padding-top: 3%;
  padding-bottom: 3%;
}
</style>
