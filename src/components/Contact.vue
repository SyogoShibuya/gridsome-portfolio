<template>
  <section class="contact-section">
    <v-container>
      <v-row>
        <v-col>
          <h1 class="text-center">Contact Information</h1>
        </v-col>
      </v-row>
      <v-row>
        <v-col sm="6" offset-sm="3" class="d-flex justify-space-around">
          <img
          class="contact-icon"
          src="https://simpleicons.org/icons/github.svg"
          >
          <img
          class="contact-icon"
          src="https://simpleicons.org/icons/pixiv.svg"
          >
          <img
          class="contact-icon"
          src="https://simpleicons.org/icons/twitter.svg"
          >
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<style>
.contact-section {
    background-color: #FFD563;
}
.contact-icon {
    height: 40px;
}
</style>