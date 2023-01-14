<template>
  <v-card
    elevation="12"
    max-width="80vw"
    class="my-8 mx-8"
    theme="dark"
  >
    <v-img :src="'~/public/' + img" max-width="800" />
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
    img: {
      default: 'acacia.png',
      type: String
    },
    name: {
      default: 'Default',
      type: String
    },
    desc: {
      default: 'Default description',
      type: String
    },
    to: {
      default: '',
      type: String
    }
  }
}
</script>
