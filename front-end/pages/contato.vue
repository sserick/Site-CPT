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
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3602.59937853175!2d-49.238018684593655!3d-25.451653983778506!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94dce51a4ba91197%3A0x66846c16d9004ed5!2sN%C3%BAcleo%20de%20Pesquisa%20e%20Desenvolvimento%20de%20Energia%20Autossustent%C3%A1vel!5e0!3m2!1spt-BR!2sbr!4v1604519859648!5m2!1spt-BR!2sbr"
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
    Inicio,
  },
  methods: {},
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
