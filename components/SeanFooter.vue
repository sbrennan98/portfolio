<template>
  <v-flex class="d-flex justify-space-between">
    <v-flex class="d-flex">
      <v-card color="rgba(255,0,0,0)" flat>
        <v-icon>mdi-email</v-icon>
        <span>Email:&nbsp;</span>
        <a href="mailto:sbrennan@mail.missouri.edu">sbrennan@mail.missouri.edu</a>
      </v-card>

      <v-card color="rgba(255,0,0,0)" flat class="mx-8">
        <v-icon>mdi-linkedin</v-icon>
        <span>LinkedIn:&nbsp;</span>
        <a href="https://linkedin.com/in/sbrennan98" target="_blank">sbrennan98</a>
      </v-card>

      <v-card color="rgba(255,0,0,0)" flat>
        <v-icon>mdi-github</v-icon>
        <span>GitHub:&nbsp;</span>
        <a href="https://github.com/sbrennan98" target="_blank">sbrennan98</a>
      </v-card>

      <!-- <span>&emsp;Portfolio:&nbsp;</span>
      <a href="https://brennans.info">brennans.info</a> -->
    </v-flex>
    <v-card color="rgba(255,0,0,0)" flat>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-card>
  </v-flex>
</template>
