<template>
  <v-layout column class="justify-center align-center">
    <FamilyMember
      img="sean.jpg"
      name="Sean Lee Brennan"
      desc="Sean studied computer science at Mizzou."
      to="/sean"
    />
    <FamilyMember
      img="maria.jpg"
      name="Maria Jose Garzon Ruiz"
      desc="Maria is a superhero."
      to=""
    />
    <!-- Making use of Vue props like above makes it so much cleaner, huh?
    <v-card
      elevation="2"
      max-width="800"
      class="my-8 mx-8"
    >
      <v-img :src="require('@/assets/sean.png')" />
      <v-card-title class="justify-center">Sean Lee Brennan</v-card-title>
      <v-card-text>
        <div>
          Sean studied computer science at Mizzou. He works at Amazon as a software development engineer. He's kinda the coolest.
        </div>
      </v-card-text>
      <v-card-actions>
        <v-btn>
          More About Me
        </v-btn>
      </v-card-actions>
    </v-card>

    <v-card
      elevation="2"
      max-width="800"
      class="my-8 mx-8"
    >
      <v-img :src="require('~/assets/maria.jpg')" />
      <v-card-title class="justify-center">Maria Jose Garzon Ruiz</v-card-title>
      <v-card-text>
        <div>
          Maria is a superhero.
        </div>
      </v-card-text>
      <v-card-actions>
        <v-btn>
          More About Me
        </v-btn>
      </v-card-actions>
    </v-card>
    -->
    <FamilyMember img="acacia.png" name="Acacia Lee Brennan-Garzon" desc="La Bebita. She enjoys ballet." />
  </v-layout>
</template>

<script>
import FamilyMember from './FamilyMember.vue'
export default {
  components: { FamilyMember }
}
</script>
