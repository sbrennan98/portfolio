<template>
  <v-app>
    <v-parallax
      src="https://insights.bcdme.com/hs-fs/hubfs/Imported_Blog_Media/Austin-ariel-view.jpg?width=3994&height=2658&name=Austin-ariel-view.jpg"
      height="auto"
    >
      <v-row
        justify="center"
        align="center"
      >
        <v-col
          class="text-center"
          justify="center"
          align="center"
        >
          <h1 class="text-h1">The Brennans</h1>
          <FamilyMembers />
        </v-col>
      </v-row>
      <Nuxt />
    </v-parallax>
  </v-app>
</template>

<script lang="ts">
export default {
  name: 'LandingPage',
  layout: 'landing'
}
</script>

<style scoped>
  h1 {
    color: black;
  }
</style>
