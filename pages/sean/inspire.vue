<template>
  <v-app>
    <v-row>
      <v-col class="text-center">
        <img
          src="https://1.bp.blogspot.com/-eeYOiXwnehw/X3Rvi4Od0RI/AAAAAAAAA4U/94PRVjVnyKUE_R5Z5B05_IJqiDK2gnA2ACLcBGAsYHQ/s1920/Albert%2BEinstein%2Bneelcrew.jpg"
          alt="Albert Einstein"
          class="mb-2"
        >
        <blockquote class="blockquote">
          &#8220;Computers are incredibly fast, accurate, and stupid. Human beings are incredibly slow, inaccurate, and brilliant. Together they are powerful beyond imagination.&#8221;
          <footer>
            <small>
              <em>&mdash;Albert Einstein</em>
            </small>
          </footer>
        </blockquote>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <h1>Resources</h1>
        <p>Here are some free online resources I've collected for topics in computer science & software engineering.</p>
      </v-col>
      <v-col>
        <v-expansion-panels multiple>
          <v-expansion-panel>
            <v-expansion-panel-header>Data Structures</v-expansion-panel-header>
            <v-expansion-panel-content>TBA</v-expansion-panel-content>
          </v-expansion-panel>
          <v-expansion-panel>
            <v-expansion-panel-header>Algorithms</v-expansion-panel-header>
            <v-expansion-panel-content>TBA</v-expansion-panel-content>
          </v-expansion-panel>
          <v-expansion-panel>
            <v-expansion-panel-header>Design Patterns</v-expansion-panel-header>
            <v-expansion-panel-content>TBA</v-expansion-panel-content>
          </v-expansion-panel>
          <v-expansion-panel>
            <v-expansion-panel-header>Prog Lang Syntax</v-expansion-panel-header>
            <v-expansion-panel-content>TBA</v-expansion-panel-content>
          </v-expansion-panel>
        </v-expansion-panels>
      </v-col>
    </v-row>
  </v-app>
</template>

<script>
export default {
  name: 'InspirePage'
}
</script>

<style scoped>
img {
    width:100%;
    max-width:600px;
}
</style>
