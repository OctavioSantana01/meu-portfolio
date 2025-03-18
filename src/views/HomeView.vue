<template>
  <v-container fluid class="fundo-home pa-0 ma-0">
    <div class="textos">
      <h1>Bem-vindo</h1>
      <p>Desenvolvedor Full Stack</p>
      <v-tooltip top>
        <template v-slot:activator="{ on, attrs }">
          <v-btn
            :loading="loading"
            rounded
            outlined
            color="#ff7f7f"
            width="15rem"
            class="mt-4"
            v-bind="attrs"
            v-on="on"
            @click="clickEvento"
            >Saiba mais</v-btn
          >
        </template>
        <span>{{ mostrarMensagemSugestao }}</span>
      </v-tooltip>
    </div>
  </v-container>
</template>

<script>
export default {
  name: "HomePage",

  data() {
    return {
      loading: false,
    };
  },

  computed: {
    mostrarMensagemSugestao() {
      return "Clique para saber mais sobre mim";
    },
  },

  methods: {
    clickEvento() {
      this.loading = true;
      setTimeout(() => {
        this.$router.push({
          name: "sobre",
        });
      }, 1000);
    },
  },
};
</script>

<style scoped>
.fundo-home {
  height: calc(100vh - 64px);
  background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url(../assets/images/portfolio.png);
  background-size: cover;
  background-position: center;
}

.textos h1,
.textos p {
  position: relative;
  z-index: 1;
  color: #fff;
  text-align: center;
}

.textos h1 {
  font-size: 2rem;
  margin-top: 10px;
  margin-right: 105px;
  font-weight: 300;
}

.textos p {
  font-size: 5rem;
  margin-top: 15px;
  margin-right: 105px;
}

.textos {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100%;
}
</style>
