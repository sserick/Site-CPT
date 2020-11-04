<template>
  <v-container class="EquipeColor">
    <v-row>
      <v-col cols="12">
        <h1 class="TitleEquipe">{{ title }}</h1>
      </v-col>
    </v-row>
    <v-row justify="center">
      <v-expansion-panels popout>
        <v-expansion-panel
          v-for="(message, i) in messages"
          :key="i"
          hide-actions
        >
          <v-expansion-panel-header class="colorExpansion">
            <v-row align="center" no-gutters>
              <v-col cols="4" sm="2" md="1">
                <v-avatar size="36px">
                  <img
                    alt="Avatar"
                    src="https://avatars0.githubusercontent.com/u/9064066?v=4&s=460"
                  />
                </v-avatar>
              </v-col>

              <v-col class="hidden" cols="8" sm="5" md="3">
                <strong v-html="message.name"></strong>
              </v-col>

              <v-col class="text-no-wrap" cols="12" sm="3">
                <strong v-html="message.title"></strong>
              </v-col>

              <v-col class="text-no-wrap" cols="12" sm="3">
                <v-row justify="space-around">
                  <v-btn icon :href="message.facebook">
                    <v-icon color="white darken-2">
                      mdi-facebook
                    </v-icon>
                  </v-btn>

                  <v-btn icon :href="message.instagram">
                    <v-icon color="white darken-2">
                      mdi-instagram
                    </v-icon>
                  </v-btn>

                  <v-btn icon :href="message.linkedln">
                    <v-icon color="white darken-2">
                      mdi-linkedin
                    </v-icon>
                  </v-btn>
                </v-row>
              </v-col>
            </v-row>
          </v-expansion-panel-header>
          <v-expansion-panel-content class="colorExpansion">
            <v-divider></v-divider>
            <v-card-text v-text="message.text"></v-card-text>
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-row>
  </v-container>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true,
      default: '',
    },
    messages: {
      type: Array,
      required: true,
      default: () => [],
    },
  },
  data() {
    return {
      hoverOne: false,
    }
  },
}
</script>

<style>
.EquipeColor {
  background-color: #10041c;
}

.TitleEquipe {
  margin-top: 10px;
  margin-left: 10px;
  color: #fcd24a;
}

.colorExpansion {
  background-color: #230c3d;
}

a {
  text-decoration: none;
  color: white;
}
</style>
