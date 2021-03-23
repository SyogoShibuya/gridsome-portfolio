<template>
  <Layout>

    <About />
    <Skills />
    <Education />
    <Contact />

  </Layout>
</template>

<script>
import About from '@/components/About.vue'
import Skills from '@/components/Skills.vue'
import Education from '@/components/Education.vue'
import Contact from '@/components/Contact.vue'

export default {
  metaInfo: {
    title: 'Hello, world!'
  },
  components: {
    About,
    Skills,
    Education,
    Contact,
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
