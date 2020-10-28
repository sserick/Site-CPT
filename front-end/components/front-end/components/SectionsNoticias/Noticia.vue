<template>
  <v-card color="#230c3d" max-width="400">
    <v-img :src="imagem" height="200px"></v-img>

    <v-card-title class="textOne">
      {{ titulo }}
    </v-card-title>

    <v-card-actions>
      <v-btn disabled icon color="white" class=" margin marginR">
        <v-icon class="iconSpaceText">mdi-eye</v-icon>
        <span>55</span>
      </v-btn>

      <v-btn icon color="pink" class="marginR" @click="counterCurtidas += 1">
        <v-icon class="iconSpaceText">mdi-heart</v-icon>
        <span>{{ counterCurtidas }}</span>
      </v-btn>

      <v-bottom-sheet v-model="sheet">
        <template v-slot:activator="{ on, attrs }">
          <v-icon v-bind="attrs" v-on="on">mdi-share-variant</v-icon>
        </template>
        <v-list color="#230c3d">
          <v-subheader>Compartilhar em</v-subheader>
          <v-list-item
            v-for="tile in tiles"
            :key="tile.title"
            @click="sheet = false"
          >
            <v-list-item-avatar>
              <v-avatar size="32px" tile>
                <img
                  :src="
                    `https://cdn.vuetifyjs.com/images/bottom-sheets/${tile.img}`
                  "
                  :alt="tile.title"
                />
              </v-avatar>
            </v-list-item-avatar>
            <v-list-item-title>{{ tile.title }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-bottom-sheet>

      <v-btn icon class="marginL" @click="show = !show">
        <v-icon>{{ show ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
      </v-btn>
    </v-card-actions>

    <v-expand-transition>
      <div v-show="show">
        <v-divider></v-divider>

        <v-card-text>
          {{ texto }}
        </v-card-text>
      </div>
    </v-expand-transition>
  </v-card>
</template>

<script>
export default {
  props: {
    titulo: {
      type: String,
      required: true,
      default: 'Título'
    },
    texto: {
      type: String,
      required: true,
      default: 'Texto da notícia'
    },
    imagem: {
      type: String,
      default: '/imagens/Icons/LogoCPT.png'
    }
  },
  data() {
    return {
      show: false,
      counterCurtidas: 0,
      sheet: false,
      tiles: [
        { img: 'keep.png', title: 'Keep' },
        { img: 'inbox.png', title: 'Inbox' },
        { img: 'hangouts.png', title: 'Hangouts' },
        { img: 'messenger.png', title: 'Messenger' },
        { img: 'google.png', title: 'Google+' }
      ]
    }
  }
}
</script>

<style>
.NoticiaColor {
  background-color: #230c3d;
}

.margin {
  margin-left: 15px;
}

.marginR {
  margin-right: 30px;
}

.marginL {
  margin-left: 7%;
}

.marginROne {
  margin-right: 20px;
}

.iconSpaceText {
  margin-right: 5px;
}

.TextImage {
  width: 400px;
  height: 500px;
}

.conteudo {
  background-color: rgba(133, 116, 150, 0.5);
  width: 400px;
}

.textOne {
  text-align: justify;
  font-size: 15px;
}

@media (min-width: 1000px) {
  .marginL {
    margin-left: 40%;
  }
}
</style>
