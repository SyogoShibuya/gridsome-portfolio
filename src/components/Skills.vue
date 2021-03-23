<template>
  <section id="skills" class="project-section">
    <v-container>
        <v-row>
            <v-col>
              <h1>Skills</h1>
              使用言語やソフトウェアなど
            </v-col>
        </v-row>
        <v-row class="justify-center mb-4">
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
                <!--
                <v-btn
                    color="orange"
                    text
                    :href="project.github"
                >
                Link
                </v-btn>
                -->
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
                  name: 'Python',
                  github: 'https://github.com/SyogoShibuya/blogsample-django',
                  description: '研究としての植物病害自動診断システム構築やインターンシップでの機械学習ソフトの作成を行っています。',
                  image: 'https://i.imgur.com/3iI6zN5.png'
              },
              {
                  name: 'Flask/Django（Python）',
                  github: 'https://github.com/SyogoShibuya/blogsample-django',
                  description: 'インターンシップや趣味でバックエンド開発を行っています。主にAIのデモページ作成に用います。',
                  image: 'https://cdn-ak.f.st-hatena.com/images/fotolife/h/hotcocoastudy/20210215/20210215132745.png'
              },
              {
                  name: 'HTML/CSS, Javascript(jQuery/Vue)',
                  github: 'https://github.com/SyogoShibuya/blogsample-django',
                  description: 'インターンシップや趣味でフロントエンド開発を行いました。本サイトもVueを用いて作成しています。',
                  image: 'https://jp.vuejs.org/images/logo.png'
              },
              {
                  name: 'C++',
                  github: 'https://github.com/SyogoShibuya/blogsample-django',
                  description: 'インターンシップ先でのアプリケーション開発を主に行っています。大学の授業でも軽く勉強しました。',
                  image: 'https://upload.wikimedia.org/wikipedia/commons/thumb/1/18/ISO_C%2B%2B_Logo.svg/144px-ISO_C%2B%2B_Logo.svg.png'
              },
              {
                  name: 'Linux',
                  github: 'https://github.com/SyogoShibuya/blogsample-django',
                  description: '研究室でDNSサーバ、Webサーバ(Nginx)、LDAPサーバ、メールサーバ、SSH設定などのサーバ構築をしました。',
                  image: 'https://cdn.worldvectorlogo.com/logos/ubuntu-2.svg'
              },
              {
                  name: 'Clip Studio Paint',
                  github: 'https://github.com/SyogoShibuya/blogsample-django',
                  description: '液晶タブレットやiPad Proでのイラスト制作。Live2Dでのモデル作成も行います。',
                  image: 'https://pbs.twimg.com/media/EbmY4DoVAAAByHL?format=jpg&name=large'
              },
              {
                  name: 'PhotoShop',
                  github: 'https://github.com/SyogoShibuya/blogsample-django',
                  description: '画像処理や簡単なWebデザインを行っています。現在勉強中です。',
                  image: 'data:image/png;base64,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'
              },
              {
                  name: 'Blender',
                  github: 'https://github.com/SyogoShibuya/Chainer-Cutmix',
                  description: 'Blenderを用いた簡単な3DCG作成。現在勉強中です。イラストの背景に使えるようなものを中心に作成しています。',
                  image: 'https://cdn-ak.f.st-hatena.com/images/fotolife/h/hotcocoastudy/20210212/20210212074356.png',
                  link: 'link',
              },
              {
                  name: 'Cubism',
                  github: 'https://github.com/SyogoShibuya/blogsample-django',
                  description: 'アプリ用のLive2Dの作成を行いました。研究室の後輩とチャットアプリの作成も行いました。',
                  image: 'https://i.imgur.com/gXI6yLk.png'
              },
              {
                  name: 'Others',
                  github: 'https://github.com/SyogoShibuya/blogsample-django',
                  description: 'Gitによる共同開発やDockerでの環境構築の経験。大学の授業でC言語、Javaの基礎を勉強しました。',
                  image: 'https://pbs.twimg.com/profile_images/1273307847103635465/lfVWBmiW_400x400.png'
              },
          ]
      }
  },
  methods: {
      truncate(str) {
          if (str.length > 60){
              return str.slice(0, 59) + '...'
          }
          return str
      }
  }
}
</script>

<style scoped>
.project-section {
    background-color: #bde8ff;
}
.v-image {
    border-bottom: 1px solid;
}
v-card {
    padding: 10px;
}
</style>