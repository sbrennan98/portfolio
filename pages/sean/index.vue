<template>
  <v-container>
    <h1>Biography</h1>
    <!-- <v-img src="https://brennans.info/_nuxt/img/sean.79a449e.jpg" alt="Sean in Houston" max-width="600" max-height="600" /> -->
    <img src="~/public/sean.jpg" />
    <v-img :src="'@/public/sean.jpg'" alt="Sean in Houston" max-width="600" max-height="600" />
    <h2>Sean Lee Brennan</h2>
    <p>Hello, my name is Sean Brennan. I graduated from the University of Missouri - Columbia (colloquially known as Mizzou) with a Bachelor of Science in Computer Science and a Minor in Mathematics. I successfully completed a software development engineering internship at Amazon in the summer of 2022 and obtained a full-time offer, just one semester before my graduation in December of 2022. However, my offer like many others was unfortunately delayed for six months until August of 2023. While I am a dedicated software engineer, I am also a dedicated father to my three-year-old daughter and a dedicated husband to my wife. Because of this, I have familial & financial obligations to fullfil and cannot afford to wait idly for half a year. If you're interested in an engineer who is obsessed with iterative improvement, don't hesitate to reach out.</p>
  </v-container>
</template>

<script>
export default {
  name: 'SeanBio'
}
</script>
