<template>
  <section id="education-experience">
    <v-container>
      <v-row>
        <v-col>
          <h1>Education & Experience</h1>
        </v-col>
      </v-row>
      <v-row>
        <v-col>
          <v-timeline>
            <v-timeline-item
            v-for="(year, i) in years"
            :key="i"
            :color="year.color"
            small
            >
            <template v-slot:opposite>
                <span
                :class="`headline font-weight-bold ${year.color}--text`"
                v-text="year.year"
                ></span>
                <div class="py-4">
                    <h2 :class="`headline font-weight-light mb-4 ${year.color}--text`">
                    {{ year.title }}
                    </h2>
                    <div>
                    {{ year.desc }}
                    </div>
                </div>
            </template>
            </v-timeline-item>
        </v-timeline>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>


<script>
  export default {
    data: () => ({
      years: [
        {
          color: 'cyan',
          year: '2020/9',
          title: '株式会社セルシス長期インターンシップ参加',
          desc: 'アプリケーション開発やイラスト支援の画像処理研究を主に行っています。',
        },
        {
          color: 'teal',
          year: '2020/4',
          title: '法政大学大学院理工学研究科応用情報工学専攻入学',
          desc: '',
        },
        {
          color: 'green',
          year: '2020/3',
          title: '法政大学理工学部応用情報工学科卒業',
          desc: '第82回情報処理学会で「中央領域に注目する Center Attention による頑健性の高い植物病害診断装置の構築」の発表を行いました。また学科主席として成績優秀賞を頂きました。',
        },
        {
          color: 'purple',
          year: '2018/11',
          title: '株式会社アーク情報システム長期インターンシップ参加',
          desc: 'AIエンジニアとして参加。物体検出やトレンド分析、異常検知などの業務に合わせた技術の調査や実装の検証などを行いました。',
        },
        {
          color: 'pink',
          year: '2016/4',
          title: '法政大学理工学部応用情報工学科入学',
          desc: '',
        },
        {
          color: 'orange',
          year: '2015/4',
          title: '千葉県立船橋芝山高等学校卒業',
          desc: '',
        },
      ],
    }),
  }
</script>