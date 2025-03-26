<template>
  <v-app>
    <v-app-bar app dark>
      <v-toolbar-title>Meu Portfólio</v-toolbar-title>
      <div class="ml-auto mr-10">
        <v-btn class="botao-rotas" text to="/">Home</v-btn>
        <v-btn class="botao-rotas" text to="/sobre">Sobre Mim</v-btn>
        <v-btn class="botao-rotas" text to="/projetos">Projetos</v-btn>
        <v-btn class="botao-rotas" text to="/contato">Contato</v-btn>
      </div>
    </v-app-bar>

    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "App",

  data: () => ({
    botaoSelecionado: null,
  }),
});
</script>
<style lang="css" scoped>
.botao-rotas:hover {
  background-color: #0070f3;
  transform: scale(1.1);
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);
}
.v-btn--active {
  background-color: #0070f3 !important;
  color: #fff;
  transform: scale(1.1);
}
</style>
