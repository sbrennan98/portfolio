<template>
  <v-col class="d-flex justify-space-between ma-0 pa-0">
    <v-col class="d-flex ma-0 pa-0 flex-wrap">
      <FooterItem 
        icon="mdi-email"
        name="Email"
        link="mailto:brennansean6@gmail.com"
        value="brennansean6@gmail.com"
      />
      <FooterItem 
        icon="mdi-linkedin"
        name="LinkedIn"
        link="https://linkedin.com/in/sbrennan98"
        value="sbrennan98"
      />
      <FooterItem 
        icon="mdi-github"
        name="GitHub"
        link="https://github.com/sbrennan98"
        value="sbrennan98"
      />

      <!-- <span>&emsp;Portfolio:&nbsp;</span>
      <a href="https://brennans.info">brennans.info</a> -->
    </v-col>
    <v-card flat>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-card>
  </v-col>
</template>
