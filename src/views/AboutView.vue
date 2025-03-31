<template>
  <v-container fluid class="pb-2">
    <v-overlay :value="loading ? 'success' : null" :disabled="loading">
      <v-progress-circular
        indeterminate
        :rotate="360"
        :size="100"
        :width="10"
        color="black"
      />
    </v-overlay>
    <v-row class="d-flex">
      <v-col cols="12" xs="12" sm="6" md="6" lg="4">
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
                <v-col md="12" sm="12" xs="12" class="d-flex justify-md-center">
                  <h2>Octávio Santana</h2>
                </v-col>
              </v-row>
              <v-row>
                <v-col md="12" sm="12" xs="12" class="d-flex justify-md-center">
                  <h3>25 Anos</h3>
                </v-col>
              </v-row>
              <v-row>
                <v-col>
                  <v-list two-line color="#dde1e7">
                    <v-list-item>
                      <v-list-item-icon>
                        <v-icon color="#0070F3"> mdi-map-marker </v-icon>
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
                  <v-divider></v-divider>
                  <v-list two-line color="#dde1e7">
                    <v-list-item>
                      <v-list-item-icon>
                        <v-icon color="#0070F3"> mdi-phone </v-icon>
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
                        <v-icon color="#0070F3"> mdi-email </v-icon>
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
                        <v-icon color="#0070F3">mdi-school </v-icon>
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
                        <v-icon color="#0070F3">mdi-code-tags </v-icon>
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
                    <v-list two-line color="#dde1e7">
                      <v-list-item>
                        <v-list-item-icon>
                          <v-icon color="#0070F3"> mdi-github </v-icon>
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
                    <v-list two-line color="#dde1e7">
                      <v-list-item>
                        <v-list-item-icon>
                          <v-icon color="#0070F3"> mdi-linkedin </v-icon>
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
      <v-col cols="12" xs="12" sm="3" md="3" lg="4">
        <div>
          <TrajetoriaView />
        </div>
      </v-col>
      <v-col cols="12" xs="12" sm="3" md="3" lg="4">
        <div>
          <ExperienciaView />
        </div>
      </v-col>
    </v-row>
    <v-row no-gutters>
      <v-col cols="12" sm="6" class="text-center text-sm-left">
        <span class="subtitle-2"
          >© {{ new Date().getFullYear() }} Octávio Santana. Todos os direitos
          reservados.</span
        >
      </v-col>
    </v-row>
  </v-container>
</template>
<script lang="ts">
import TrajetoriaView from "@/views/Trajetoria.vue";
import Vue from "vue";
import ExperienciaView from "./ExperienciaView.vue";
export default Vue.extend({
  name: "AboutPage",

  components: {
    TrajetoriaView,
    ExperienciaView,
  },
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
});
</script>
<style scoped>
.scroll-card {
  scrollbar-width: thin;
  overflow-y: auto;
  overflow-x: hidden;
  max-width: 500px;
  background-color: #dde1e7;
  border-radius: 20px;
  padding: 2rem;
  max-height: calc(100vh - 73px);
  height: 100%;
}
</style>
