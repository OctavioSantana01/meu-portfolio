<template>
  <v-card class="card-sobre scroll-card-trajetoria">
    <h3 class="titulo-card mb-4">Minha Trajetória</h3>
    <v-divider></v-divider>
    <p class="texto-trajetoria mt-4">
      Olá! Sou Octávio Santana, tenho 25 anos, graduado em Ciência da Computação
      e pós-graduando em Engenharia de Software. Sou um Desenvolvedor Full Stack
      apaixonado por criar soluções tecnológicas que resolvem problemas reais.
      Com 4 anos de de experiência no desenvolvimento de aplicações, tenho
      focado em construir interfaces intuitivas e códigos robustos.
    </p>
    <p class="mt-4 texto-trajetoria">
      Minha jornada na programação começou durante meu curso de Ciência da
      Computação, em 2019, e foi na PUC MINAS campus Poços de Caldas onde
      descobri minha paixão por transformar linhas de código em experiências
      significativas. Desde então,venho aprimorando constantemente técnicas e
      soft skills para entregar projetos de alta qualidade.
    </p>
    <p class="mt-5 texto-trajetoria">
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
  height: 650px;
  width: 450px;
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
.texto-trajetoria {
  font-weight: 300;
  font-size: 1rem;
  color: #ffffff;
}
</style>
