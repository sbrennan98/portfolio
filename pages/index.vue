<template>
    <v-parallax
        src="https://images.pexels.com/photos/18583619/pexels-photo-18583619.jpeg"
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
