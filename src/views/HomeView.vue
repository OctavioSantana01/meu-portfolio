<template>
  <v-container fluid class="fundo-home pa-0 ma-0">
    <div class="fundo-transparente">
      <h1>Bem-vindo</h1>
      <p>Desenvolvedor Full Stack</p>
    </div>
  </v-container>
</template>

<script>
export default {
  name: "HomePage",
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
.fundo-transparente h1,
.fundo-transparente p {
  position: relative;
  z-index: 1;
  color: #fff;
  text-align: center;
}
.fundo-transparente h1 {
  font-size: 2rem;
  margin-top: 10px;
  margin-right: 105px;
  font-weight: 300;
}

.fundo-transparente p {
  font-size: 5rem;
  margin-top: 15px;
  margin-right: 105px;
}
.fundo-transparente {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100%;
}
</style>
