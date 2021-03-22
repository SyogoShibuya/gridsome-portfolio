<template>
  <Layout>

    <section>
      <v-container>
        <v-row>
          <v-col>
            <g-image alt="Example image" src="~/profile.jpg" width="400" />
          </v-col>
          <v-col sm="6">
            <h1>澁谷将吾</h1>
            <p>法政大学理工学研究科応用情報工学専攻１年</p>
          </v-col>
        </v-row>
      </v-container>
    </section>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Hello, world!'
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
