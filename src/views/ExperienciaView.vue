<template>
  <v-card class="card-sobre scroll-card-trajetoria">
    <h3 class="titulo-card mb-2">Experiências Profissionais</h3>
    <v-card
      v-for="(exp, index) in experiences"
      :key="index"
      @mouseover="hover = true"
      @mouseleave="hover = false"
      class="experience-card mt-4"
      hover
      color="#dde1e7"
      elevation="2"
      :style="{ animationDelay: `${index * 150}ms` }"
    >
      <v-card-title class="pb-0">
        <h3 class="text-h6">{{ exp.titulo }}</h3>
      </v-card-title>
      <v-card-subtitle class="pt-2">
        <div class="d-flex align-center mt-2">
          <v-icon color="#2E8AF5"> mdi-domain </v-icon>
          <span class="font-weight-medium ml-1">{{ exp.empresa }}</span>
          <v-icon color="#2E8AF5" class="ml-2"> mdi-calendar-range </v-icon>
          <v-chip x-small outlined class="ml-1">{{ exp.duracao }}</v-chip>
        </div>
      </v-card-subtitle>
      <v-card-text>
        <p class="mb-3 texto-descricao">{{ exp.descricao }}</p>
        <v-divider></v-divider>
        <h4 class="mt-2">Habilidades Utilizadas</h4>
        <div class="d-flex flex-wrap">
          <v-chip
            v-for="skill in exp.skills"
            :key="skill"
            x-small
            class="mr-1 mb-1 mt-2"
            color="#2E8AF5"
            outlined
          >
            {{ skill }}
          </v-chip>
        </div>
      </v-card-text>
    </v-card>
  </v-card>
</template>
<script>
import Vue from "vue";
export default Vue.extend({
  name: "ExperienciaView",

  data() {
    return {
      hover: false,
    };
  },
  computed: {
    experiences() {
      return [
        {
          titulo: "Desenvolvedor Full Stack",
          empresa: "Grupo Soitic",
          duracao: "2021-2023",
          descricao:
            "Atuava utilizando o Builder 6, utilizando a linguagem de programação C++, linguagem de consulta SQL e banco de dados SQL SERVER, também utiliza o Delphi 7, utilizando a linguagem de programação Delphi.",
          skills: [
            "Builder 6",
            "C++",
            "SQL",
            "Delphi 7",
            "Delphi 6",
            "SQL SERVER",
            "Git",
          ],
        },
        {
          titulo: "Desenvolvedor Full Stack",
          empresa: "Grupo Soitic",
          duracao: "2024-Atual",
          descricao:
            "Atuo como desenvolvedor Full Stack, focando em tecnologias como Vue.js, TypeScript, Node.js e .Net. Minha experiência inclui o desenvolvimento de aplicações, com ênfase em design responsivo e usabilidade.",
          skills: [
            "Vue.js",
            "TypeScript",
            "Node.js",
            ".Net",
            "Design Responsivo",
            "Solid",
          ],
        },
      ];
    },
  },
});
</script>
<style scoped>
.card-sobre {
  background-color: #6f859b;
  border-radius: 20px;
  padding: 2rem;
  height: 650px;
  width: 700px;
  text-align: center;
}
.scroll-card-trajetoria {
  scrollbar-width: thin;
  overflow-y: auto;
  overflow-x: hidden;
}

.card-sobre:hover {
  transform: translateY(-15px);
}
.titulo-card {
  font-size: 1.5rem;
  font-weight: 500;
  color: "black";
}
.experience-card {
  background-color: #fafafa;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.experience-card:hover {
  transform: translateY(-5px);
}
.texto-descricao {
  font-weight: 300;
  font-size: 1rem;
  color: #000000;
  align-items: center;
  text-align: left;
  margin: 0;
  padding: 0;
  line-height: 1.5;
  max-height: 100px;
  overflow: hidden;
  text-overflow: ellipsis;
}
.experience-card:hover .v-chip {
  background-color: #2e8af5 !important;
  color: #fff !important;
}
</style>
