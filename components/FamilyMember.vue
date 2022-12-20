<template>
  <v-card
    elevation="2"
    max-width="800"
    class="my-8 mx-8"
  >
    <v-img :src="require('@/assets/' + img)" />
    <v-card-title class="justify-center">
      {{ name }}
    </v-card-title>
    <v-card-text>
      <div>
        {{ desc }}
      </div>
    </v-card-text>
    <v-card-actions>
      <v-btn :to="to">
        More About Me
      </v-btn>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {
  props: {
    img: String,
    name: String,
    desc: String,
    to: String
  }
}
</script>
