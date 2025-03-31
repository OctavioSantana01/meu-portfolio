<template>
  <v-card class="card-sobre scroll-card-trajetoria">
    <h3 class="titulo-card mb-4">Experiências Profissionais</h3>
    <v-divider></v-divider>
  </v-card>
</template>
<script>
export default {
  name: "ExperienciaView",
};
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
</style>
