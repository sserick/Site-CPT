<template>
  <v-container-fluid class="MVVColor">
    <v-row>
      <v-card color="#3fa944" class="cardImage"> </v-card>
    </v-row>
  </v-container-fluid>
</template>

<script>
export default {}
</script>

<style scoped>
.ImageSizeOne {
  height: 650px;
  width: 100%;
}

.ImageSize {
  height: 450px;
  width: 100%;
}

.cardImage {
  background-image: url('/imagens/Fundos/CPTBio.JPG');
  height: 650px;
  background-attachment: fixed;
  background-repeat: no-repeat;
  background-size: 200% 750px;
  background-position: center;
}

.MVVColor {
  background-color: #151626;
}

@media (min-width: 701px) and (max-width: 958px) {
  .ImageSize {
    height: 250px;
    width: 100%;
  }
}

@media (min-width: 920px) and (max-width: 2000px) {
  .cardImage {
    width: 100%;
    height: 650px;
    background-size: 100% 100%;
  }
}
</style>
