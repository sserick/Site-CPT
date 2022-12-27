<template>
  <v-container-fluid class="NoticiaColor">
    <div class="imagem">
      <div class="overflow">
        <v-row
          class="align"
          justify="center"
          align="center"
          style="height: 100%;"
        >
          <h1 class="mb-4 fontFami font-weight-black">
            {{ titulo }}
          </h1>
        </v-row>
      </div>
    </div>
  </v-container-fluid>
</template>

<script>
export default {
  props: {
    titulo: {
      type: String,
      required: true,
      default: 'Título',
    },
  },
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

.overflow {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 600px;
}

.align {
  display: flex;
  flex-direction: column;
}

.fontFami {
  font-family: 'Trebuchet MS', sans-serif;
  color: white;
  text-align: center;
  font-size: 75px;
  margin-top: 7%;
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
