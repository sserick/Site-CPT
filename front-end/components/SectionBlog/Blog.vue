<template>
  <v-container fluid class="SectionBlog">
    <v-row align="center" justify="center">
      <v-col cols="10">
        <h1 class="TitleBlog">{{ title }}</h1>
      </v-col>
    </v-row>
    <v-row align="center" justify="center">
      <v-col
        v-for="item in blog"
        :key="item"
        cols="10"
        sm="5"
        lg="3"
        xl="3"
        class="SectionBlogText marginTop"
      >
        <v-row row align="center" justify="center">
          <img height="120" width="100%" contain :src="item.imgFundo" />
          <img
            height="90"
            width="90"
            :src="item.imgPerson"
            class="ImgRedoBlog"
          />
        </v-row>
        <v-row align="center" justify="start">
          <h3 class="titleBlog">{{ item.title }}</h3>
          <p class="textBlog">
            {{ item.date }}
          </p>
        </v-row>
        <v-row align="center" justify="center">
          <p class="textBlog">
            {{ item.text }}
          </p>
        </v-row>
        <v-row align="center" justify="end" class="buttonPadBlog">
          <v-btn
            class="ma-2 buttonSeta animationButtonBlog"
            outlined
            small
            fab
            :to="item.link"
          >
            <v-icon>mdi-arrow-right</v-icon>
          </v-btn>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  props: {
    blog: {
      type: Object,
      required: true,
      default: () => {
        return {}
      },
    },
    title: {
      type: String,
      required: true,
      default: () => {
        return {}
      },
    },
  },
  data() {
    return {
      page: 1,
    }
  },
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@600&display=swap');

.SectionBlog {
  padding-top: 3%;
  padding-bottom: 2%;
  background-color: RGBA(63, 169, 68, 0.05);
}

.TitleBlog {
  text-align: left;
  font-size: 36px;
  padding-bottom: 30px;
  font-weight: 900;
  font-family: 'Open Sans', sans-serif;
  color: #3fa944;
}

.SectionBlogText {
  border-right: solid 1px #c0c0c0;
  border-bottom: solid 1px #c0c0c0;
  box-shadow: 5px 5px 5px 0px #c0c0c0;
  border-radius: 10px;
  background-color: white;
  padding-top: 0;
  float: right;
  position: relative;
  margin-right: 2%;
  margin-bottom: 3%;
}

.ImgRedoBlog {
  border-radius: 70px;
  position: absolute;
  top: 20%;
  right: 10%;
  border-color: white;
  border-width: 1px;
  border-style: solid;
}

.titleBlog {
  text-align: left;
  font-size: 20px;
  padding-top: 50px;
  padding-left: 20px;
  padding-right: 20px;
  padding-bottom: 10px;
  font-family: 'Open Sans', sans-serif;
  color: #3c424f;
}

.textBlog {
  text-align: left;
  font-size: 14px;
  padding-bottom: 10px;
  margin-bottom: 0;
  color: #3c424f;
  padding-left: 20px;
  padding-right: 20px;
}

.buttonPadBlog {
  padding-right: 20px;
}

.buttonSeta {
  color: #3fa944;
}

.buttonSeta:hover {
  background-color: #3fa944;
  color: white;
}

.animationButtonBlog:hover {
  transform: translateX(0px) scale(1.2);
}

.buttonBlog {
  width: 150px;
  margin-top: 50px;
  color: #3fa944;
}

.buttonBlog:hover {
  background-color: #52bbeb;
  color: white;
}

@media (min-width: 768px) and (max-width: 1280px) {
  .paddingBlog {
    padding-left: 0px;
  }

  .marginTop {
    margin-top: 2%;
  }
}

@media (max-width: 767px) {
  .paddingBlog {
    padding-left: 0px;
  }

  .marginTop {
    margin-top: 2%;
  }
}
</style>
