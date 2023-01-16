<template>
  <v-card
    class="ma-8"
    theme="dark"
    width="100%"
    max-width="800"
  >
    <v-img :src="'/' + img" />
    
    <v-card-title>
      {{ name }}
    </v-card-title>
    <v-card-text>
      <div>
        {{ desc }}
      </div>
    </v-card-text>

    <v-card-actions>
      <v-btn :to="to" variant="tonal">
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
