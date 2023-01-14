<template>
    <v-parallax
        src="https://insights.bcdme.com/hs-fs/hubfs/Imported_Blog_Media/Austin-ariel-view.jpg?width=3994&height=2658&name=Austin-ariel-view.jpg"
        height="auto"
      >
        <v-row>
          <v-col class="text-center">
            <h1 class="text-h1">
              The Brennans
            </h1>
            <FamilyMembers />
          </v-col>
        </v-row>
    </v-parallax>
</template>
  
<script setup>
    definePageMeta({
        layout: 'landing'
    })
</script>
  
<style scoped>
    h1 {
      color: black;
    }
</style>
