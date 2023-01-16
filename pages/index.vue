<template>
    <v-parallax
        src="https://insights.bcdme.com/hs-fs/hubfs/Imported_Blog_Media/Austin-ariel-view.jpg?width=3994&height=2658&name=Austin-ariel-view.jpg"
        height="100%"
    >
        <v-container fluid class="text-center">
            <h2 class="text-h2">The Brennans</h2>
            <FamilyMembers />
        </v-container>
    </v-parallax>
</template>
  
<script setup>
    definePageMeta({
        layout: 'landing'
    })
</script>
