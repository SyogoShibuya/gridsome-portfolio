<template>
  <section class="project-section">
    <v-container>
        <v-row>
            <v-col>
              <h1>Projects</h1>
            </v-col>
        </v-row>
        <v-row class="justify-space-around mb-4">
            <v-card
                v-for="project in projects"
                :key="project.name"
                class=""
                max-width="300"
            >
                <v-img
                class="align-end"
                height="200px"
                :src="project.image"
                >
                </v-img>
                <v-card-title> {{ project.name }} </v-card-title>

                <v-card-text class="text--primary">
                  {{ truncate(project.description) }}                
                </v-card-text>
                <v-card-actions>
                <v-btn
                    color="orange"
                    text
                    :href="project.github"
                >
                Github Repo
                </v-btn>
                </v-card-actions>
            </v-card>
        </v-row>
    </v-container>
  </section>
</template>


<script>
export default {
  data() {
      return {
          projects: [
              {
                  name: 'CutMix',
                  github: 'https://github.com/SyogoShibuya/Chainer-Cutmix',
                  description: 'ChainerでのCutMix実装',
                  image: 'https://camo.githubusercontent.com/28c7c82731f00693564dbb9fbdb710669e6a69780ac2b3e45b1703c30ddc3698/68747470733a2f2f692e696d6775722e636f6d2f623874684a43342e706e67'
              },
              {
                  name: 'Django-Blog',
                  github: 'https://github.com/SyogoShibuya/blogsample-django',
                  description: 'Djangoを使った簡単なBlog実装a',
                  image: 'https://cdn-ak.f.st-hatena.com/images/fotolife/h/hotcocoastudy/20210215/20210215132745.png'
              }
          ]
      }
  },
  methods: {
      truncate(str) {
          if (str.length > 50){
              return str.slice(0, 49) + '...'
          }
          return str
      }
  }
}
</script>

<style scoped>
.project-section {
    background-color: #FFD563;
}
.v-image {
    border-bottom: 1px solid;
}
</style>