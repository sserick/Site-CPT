<template>
  <v-container-fluid class="CarrosselColor">
    <v-carousel
      class="margin"
      cycle
      height="100"
      hide-delimiter-background
      show-arrows-on-hover
    >
      <v-carousel-item v-for="(noticia, i) in noticias" :key="i">
        <v-sheet color="#230c3d" height="100%">
          <v-row class="align" align="center" justify="center">
            <div class="color">
              <a :href="href[i]">{{ noticia }}</a>
            </div>
          </v-row>
        </v-sheet>
      </v-carousel-item>
    </v-carousel>
  </v-container-fluid>
</template>

<script>
export default {
  data() {
    return {
      noticias: [
        'Notícia 1: Laboratório de microalgas',
        'Notícia 2: Curso de criação de Startup',
        'Notícia 3: Climoscópio',
        'Notícia 4: Bike lab',
        'Notícia 5: Semana acadêmica',
      ],
      href: ['/noticia1', '/noticia2', '/noticia3', '/noticia4', '/noticia5'],
    }
  },
}
</script>

<style scoped>
.color {
  font-size: 25px;
  font-family: 'Arapey', 'Montserrat';
}

.CarrosselColor {
  background-color: #50116e;
}

a {
  text-decoration: none;
  color: white;
}

@media screen and (max-width: 767px) {
  .color {
    font-size: 18px;
  }
}
</style>
