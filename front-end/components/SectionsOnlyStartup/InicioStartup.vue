<template>
  <v-container-fluid class="NoticiaColor">
    <div class="imagem"></div>
  </v-container-fluid>
</template>

<script>
export default {
  props: {},
}
</script>

<style scoped>
.ImageSize {
  height: 300px;
  width: 600px;
}

.imagem {
  background-attachment: fixed;
  background-repeat: no-repeat;
  background-size: contain;
  background-position: center;
  background-image: url('/imagens/Fundos/1876.jpg');
  height: 700px;
  background-color: white;
  opacity: 80%;
}

.NoticiaColor {
  background-color: #151626;
}

@media screen and (max-width: 464px) {
  .imagem {
    height: 600px;
    background-size: 600px 600px;
  }
}

@media (min-width: 465px) and (max-width: 700px) {
  .imagem {
    height: 700px;
    background-size: 800px 700px;
  }
}

@media (min-width: 701px) and (max-width: 958px) {
  .imagem {
    height: 600px;
    background-size: 1000px 700px;
  }
}

@media (min-width: 959px) and (max-width: 1305px) {
  .imagem {
    height: 600px;
    background-size: 1300px 1200px;
  }
}
</style>
