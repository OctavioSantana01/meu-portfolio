<template>
  <v-card class="card-sobre">
    <h3 class="text-h5 mb-4">Minha Trajetória</h3>
    <p>
      Olá! Sou Octávio Santana, um Desenvolvedor Full Stack apaixonado por criar
      soluções tecnológicas que resolvem problemas reais. Com 4 anos de de
      experiência no desenvolvimento de aplicações, tenho focado em construir
      interfaces intuitivas e códigos robustos.
    </p>
    <p class="mt-4">
      Minha jornada na programação começou durante meu curso de Ciência da
      Computação, em 2019, e foi na PUC MINAS campus Poços de Caldas onde
      descobri minha paixão por transformar linhas de código em experiências
      significativas. Desde então,venho aprimorando constantemente técnicas e
      soft skills para entregar projetos de alta qualidade.
    </p>
    <p class="mt-5">
      Atualmente, estou focado em tecnologias modernas como Vue.js, TypeScript,
      Node.js e .Net, sempre buscando implementar as melhores práticas de
      desenvolvimento e design.
    </p>
  </v-card>
</template>
<script>
export default {
  name: "TrajetoriaView",
};
</script>
<style scoped>
.card-sobre {
  background-color: #6f859b;
  border-radius: 20px;
  padding: 2rem;
  height: 600px;
  width: 500px;
  text-align: center;
  color: white;
}
.card-sobre:hover {
  transform: translateY(-5px);
}
</style>
