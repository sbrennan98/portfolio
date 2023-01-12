<template>
  <!-- Making use of Vue props like this gives cleaner code! -->
  <v-layout wrap column align-center justify-center>
    <FamilyMember
      img="sean.jpg"
      name="Sean Lee Brennan"
      desc="Sean studied computer science at Mizzou."
      to="/sean/bio"
    />
    <FamilyMember
      img="maria.jpg"
      name="Maria Jose Garzon Ruiz"
      desc="Maria is a superhero."
      to=""
    />
    <FamilyMember
      img="acacia.png"
      name="Acacia Lee Brennan-Garzon"
      desc="La Bebita. She enjoys ballet."
    />
  </v-layout>
</template>

<script>
import FamilyMember from './FamilyMember.vue'
export default {
  components: { FamilyMember }
}
</script>
