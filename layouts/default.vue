<template>
  <v-app>
    <Navbar />
    <v-container class="mt-5" fluid>
      <nuxt />
    </v-container>
    <Footer />
  </v-app>
</template>

<script>
import Navbar from '~/components/Navbar'
import Footer from '~/components/Footer'
export default {
  components: {
    Navbar,
    Footer
  }
}
</script>
