<template>
  <v-container fluid class="pa-0">
    <v-overlay :value="loading ? 'success' : null" :disabled="loading">
      <v-progress-circular
        indeterminate
        :rotate="360"
        :size="100"
        :width="10"
        color="black"
      />
    </v-overlay>
    <v-row>
      <v-col cols="9" md="6" sm="9" xs="12">
        <v-sheet rounded shaped>
          <v-card class="scroll-card">
            <v-card-text>
              <v-row>
                <v-col md="12" sm="12" xs="12" class="d-flex justify-md-center">
                  <v-avatar color="success" size="8rem">
                    <img :src="require('@/assets/images/perfil.png')" />
                  </v-avatar>
                </v-col>
              </v-row>
              <v-row>
                <v-col class="d-flex justify-md-center">
                  <h2>Octávio Santana</h2>
                </v-col>
              </v-row>
              <v-row>
                <v-col class="d-flex justify-md-center">
                  <h3>25 Anos</h3>
                </v-col>
              </v-row>
              <v-row>
                <v-col>
                  <v-list two-line color="customGray">
                    <v-list-item>
                      <v-list-item-icon>
                        <v-icon color="black"> mdi-map-marker </v-icon>
                      </v-list-item-icon>
                      <v-list-item-content>
                        <v-list-item-title>
                          {{ "Cidade" }}
                        </v-list-item-title>
                        <v-list-item-subtitle>
                          {{ "Passos/MG" }}
                        </v-list-item-subtitle>
                      </v-list-item-content>
                    </v-list-item>
                  </v-list>
                  <v-divider inset></v-divider>
                  <v-list two-line color="customGray">
                    <v-list-item>
                      <v-list-item-icon>
                        <v-icon color="black"> mdi-phone </v-icon>
                      </v-list-item-icon>

                      <v-list-item-content>
                        <v-list-item-title>
                          {{ "Celular" }}
                        </v-list-item-title>
                        <v-list-item-subtitle>
                          {{ "(35) 999255990" }}
                        </v-list-item-subtitle>
                      </v-list-item-content>
                    </v-list-item>
                    <v-divider></v-divider>
                    <v-list-item>
                      <v-list-item-icon>
                        <v-icon color="black"> mdi-email </v-icon>
                      </v-list-item-icon>

                      <v-list-item-content>
                        <v-list-item-title>
                          {{ "E-mail" }}
                        </v-list-item-title>
                        <v-list-item-subtitle>
                          {{ "octaviossantana@gmail.com" }}
                        </v-list-item-subtitle>
                      </v-list-item-content>
                    </v-list-item>
                    <v-divider></v-divider>
                    <v-list-item>
                      <v-list-item-icon>
                        <v-icon color="black">mdi-school </v-icon>
                      </v-list-item-icon>

                      <v-list-item-content>
                        <v-list-item-title>
                          {{ "Formação" }}
                        </v-list-item-title>
                        <v-list-item-subtitle>
                          {{ "Bacharel em Ciência da Computação" }}
                        </v-list-item-subtitle>
                        <v-list-item-subtitle>
                          {{ "Pós Graduando em Engenharia de Software" }}
                        </v-list-item-subtitle>
                      </v-list-item-content>
                    </v-list-item>
                    <v-divider></v-divider>
                    <v-list-item>
                      <v-list-item-icon>
                        <v-icon color="black">mdi-code-tags </v-icon>
                      </v-list-item-icon>

                      <v-list-item-content>
                        <v-list-item-title>
                          {{ "Área de Atuação" }}
                        </v-list-item-title>
                        <v-list-item-subtitle>
                          {{ "Desenvolvedor Full Stack" }}
                        </v-list-item-subtitle>
                      </v-list-item-content>
                    </v-list-item>
                    <v-divider></v-divider>
                    <v-list two-line color="customGray">
                      <v-list-item>
                        <v-list-item-icon>
                          <v-icon color="black"> mdi-github </v-icon>
                        </v-list-item-icon>
                        <v-list-item-content>
                          <v-list-item-title>
                            {{ "Github" }}
                          </v-list-item-title>
                          <v-list-item-subtitle>
                            <a
                              href="https://github.com/OctavioSantana01"
                              target="_blank"
                              rel="noopener"
                              style="color: inherit; text-decoration: none"
                            >
                              OctavioSantana01(Pessoal)
                            </a>
                          </v-list-item-subtitle>
                          <v-list-item-subtitle>
                            <a
                              href="https://github.com/OctavioSantanasoitic"
                              target="_blank"
                              rel="noopener"
                              style="color: inherit; text-decoration: none"
                            >
                              OctavioSantanasoitic(Profissional)
                            </a>
                          </v-list-item-subtitle>
                        </v-list-item-content>
                      </v-list-item>
                      <v-divider></v-divider>
                    </v-list>
                    <v-list two-line color="customGray">
                      <v-list-item>
                        <v-list-item-icon>
                          <v-icon color="black"> mdi-linkedin </v-icon>
                        </v-list-item-icon>
                        <v-list-item-content>
                          <v-list-item-title>
                            {{ "Linkedin" }}
                          </v-list-item-title>
                          <v-list-item-subtitle>
                            <a
                              href="https://www.linkedin.com/in/octavio-santana-6003141a7/"
                              target="_blank"
                              rel="noopener"
                              style="color: inherit; text-decoration: none"
                            >
                              Octavio Santana
                            </a>
                          </v-list-item-subtitle>
                        </v-list-item-content>
                      </v-list-item>
                    </v-list>
                  </v-list>
                </v-col>
              </v-row>
            </v-card-text>
          </v-card>
        </v-sheet>
      </v-col>
      <v-col cols="3" md="6" sm="3" xs="12">
        <v-card class="scrollable-card">
          <h1>Bem-vindo</h1>
          <p>Desenvolvedor Full Stack</p>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>
<script>
export default {
  name: "AboutPage",

  data() {
    return {
      loading: true,
    };
  },
  mounted() {
    setTimeout(() => {
      this.loading = false;
    }, 1000);
  },
};
</script>
<style scoped>
.scroll-card {
  scrollbar-width: thin;
  overflow-y: auto;
  overflow-x: hidden;
  height: 900px;
  width: 500px;
  background-color: #dde1e7;
  border-radius: 20px;
  padding: 2rem;
}
</style>
