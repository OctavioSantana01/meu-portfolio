<template>
  <v-app>
    <v-app-bar app dark>
      <v-toolbar-title>Meu Portfólio</v-toolbar-title>
      <div class="ml-auto mr-10">
        <v-btn text to="/">Home</v-btn>
        <v-btn text to="/sobre">Sobre Mim</v-btn>
        <v-btn text to="/projetos">Projetos</v-btn>
        <v-btn text to="/contato">Contato</v-btn>
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
    //
  }),
});
</script>
