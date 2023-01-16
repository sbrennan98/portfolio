<template>
  <!-- Making use of Vue props like this gives cleaner code! -->
    <v-container fluid fill-height>
        <v-row>
            <v-col class="d-flex justify-center">
                <FamilyMember
                    img="sean.jpg"
                    name="Sean Lee Brennan"
                    desc="Sean studied computer science at Mizzou."
                    to="/sean"
                />
            </v-col>
        </v-row>
        <v-row>
            <v-col class="d-flex justify-center">
                <FamilyMember
                    img="maria.jpg"
                    name="Maria Jose Garzon Ruiz"
                    desc="Maria is a superhero."
                    to=""
                />
            </v-col>
        </v-row>
        <v-row>
            <v-col class="d-flex justify-center">
                <FamilyMember
                    img="acacia.png"
                    name="Acacia Lee Brennan-Garzon"
                    desc="La Bebita. She enjoys ballet."
                />
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
import FamilyMember from './FamilyMember.vue'
export default {
  components: { FamilyMember }
}
</script>
