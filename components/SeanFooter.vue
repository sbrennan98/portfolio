<template>
  <v-flex align-self-end class="d-flex justify-space-between text-center">
    <v-card color="rgba(255,0,0,0)" flat>
      <v-icon>mdi-email</v-icon>
      <span>Email:&nbsp;</span>
      <a href="mailto:sbrennan@mail.missouri.edu">sbrennan@mail.missouri.edu</a>
      <span>&emsp;</span>

      <v-icon>mdi-link</v-icon>
      <span>LinkedIn:&nbsp;</span>
      <a href="https://linkedin.com/in/sbrennan98" target="_blank">sbrennan98</a>
      <span>&emsp;</span>

      <v-icon>mdi-github</v-icon>
      <span>GitHub:&nbsp;</span>
      <a href="https://github.com/sbrennan98" target="_blank">sbrennan98</a>

      <!-- <span>&emsp;Portfolio:&nbsp;</span>
      <a href="https://brennans.info">brennans.info</a> -->
    </v-card>
    <v-card color="rgba(255,0,0,0)" flat>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-card>
  </v-flex>
</template>

<style scoped>
v-card {
    background: none;
}
</style>
