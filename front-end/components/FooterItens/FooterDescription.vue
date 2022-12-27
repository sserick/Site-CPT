<template>
  <div class="footer-bg">
    <footer class="footer">
      <div class="footer__group">
        <div class="footer__group__item">
          <a :href="addressLink" target="_blank">
            <v-icon aria-label="Endereço da loja">
              mdi-map-marker
            </v-icon>
            {{ address }}
          </a>
        </div>
        <p class="footer__group__item">
          <v-icon aria-label="Telefone da loja">
            mdi-phone
          </v-icon>
          {{ phone }}
        </p>
      </div>
      <div class="footer__group">
        <p class="footer__group__item">
          <v-icon aria-label="E-mail da loja">
            mdi-email-outline
          </v-icon>
          {{ email }}
        </p>
        <div class="footer__group__item">
          <a :href="facebookLink" target="_blank">
            <v-icon aria-label="Perfil do Facebook">
              mdi-facebook
            </v-icon>
            {{ facebook }}
          </a>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      address:
        'Francisco H dos Santos, S/N Centro Politécnico, Setor de Tecnologia - Jardim das Américas, Curitiba - PR, 81531-990',
      addressLink: 'https://goo.gl/maps/zQD1v7d4emuASoqf8',
      phone: '(41) 3361-3432',
      email: 'cptufpr@gmail.com',
      facebook: 'cptufpr',
      facebookLink: 'https://www.facebook.com/cienciaufpr/',
    }
  },
}
</script>

<style lang="scss" scoped>
.footer-bg {
  background-color: white;
}
.footer {
  max-width: 1440px;
  margin: 0 auto;
  place-content: center;
  padding: 30px 150px;
  text-align: center;
  display: flex;
  flex-wrap: wrap;

  &__group {
    flex: 1;
    display: inline-flex;
    flex-wrap: wrap;
    flex-direction: row;
    align-items: center;

    &__item {
      flex: 1;
      min-width: 250px;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    &__item:hover a,
    &__item:hover a i.v-icon.v-icon {
      color: #3fa944;
    }
  }
}

i.v-icon.v-icon {
  color: #3fa944;
}

a {
  color: inherit;
  text-decoration: inherit;
}
</style>
