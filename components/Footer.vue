<template>
  <v-footer
    padless
  >
    <v-card
      class="flex"
      flat
      tile
    >
      <v-card-title class="red lighten-1">
        <strong class="subheading">N'hésitez pas à me contacter !</strong>

        <v-spacer></v-spacer>

        <v-btn
          v-for="social in socials"
          :key="social.name"
          :href="social.route"
          target="_blank"
          class="mx-4"
          dark
          icon
        >
          <v-icon size="24px">{{ social.icon }}</v-icon>
        </v-btn>
      </v-card-title>

      <v-card-text class="py-2 white--text text-center">
        {{ new Date().getFullYear() }} — <strong>Titouan Galvani</strong>
      </v-card-text>
    </v-card>  </v-footer>
</template>

<script>
  export default {
    data () {
      return {
        socials: [
          { name: 'Facebook', route: 'https://www.facebook.com/titouan.galvani', icon: 'fab fa-facebook' },
          { name: 'Twitter', route: 'https://twitter.com/ImMyst_', icon: 'fab fa-twitter' },
          { name: 'LinkedIn', route: 'https://www.linkedin.com/in/titouan-galvani/', icon: 'fab fa-linkedin' }
        ]
      }
    }
  }
</script>