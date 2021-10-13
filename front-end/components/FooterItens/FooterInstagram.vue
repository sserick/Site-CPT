<template>
  <div class="charming-pre-footer-bg">
    <div class="charming-pre-footer">
      <div class="about">
        <div>
          <b>
            <p class="about__title">Conheça o Ciência para Todos</p>
          </b>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Aut quae
            laboriosam vero, nostrum dele Lorem ipsum dolor sit amet consectetur
            adipisicing elit. Aut quae laboriosam vero, nostrum dele Lorem ipsum
            dolor sit amet consectetur adipisicing elit. Aut quae laboriosam
            vero, nostrum dele
          </p>
        </div>
      </div>

      <div>
        <p><v-icon color="black">mdi-instagram</v-icon> cptufpr</p>
        <div class="insta__grid">
          <div></div>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
}
</script>

<style lang="scss" scoped>
.charming-pre-footer-bg {
  background-color: #3fa944;
}

.charming-pre-footer {
  margin: 0 auto;
  max-width: 1440px;
  display: flex;
  flex-wrap: wrap;
  padding: clamp(20px, 10vw, 60px) 0;
}
.charming-pre-footer > div {
  flex: 1;
  min-width: 290px;
  text-align: center;
}

.about {
  padding: 0 clamp(10px, 8%, 50px);
  display: flex;
  flex-direction: row;
  align-items: center;
}

.about__title {
  color: white;
  font-size: 20px;
}

@media (min-width: 1024px) {
  .wrapper {
    padding-right: clamp(10px, 10vw, 150px);
    padding-left: clamp(10px, 10vw, 150px);
  }
  .about {
    border-right: 2px solid white;
  }
}

.insta__grid {
  display: grid;
  grid-template: repeat(3, 100px) / repeat(3, 100px);
  place-content: center;

  & > div {
    background-color: lightgrey;
    margin: 2px;
  }
}
</style>
