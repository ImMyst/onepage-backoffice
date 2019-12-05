<template>
  <v-carousel :cycle="true" :show-arrows="false">
    <v-carousel-item v-for="image in images" :key="image" :src="image">
    </v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
    data () {
      return {
        images: [
          'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg',
          'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
        ],
      }
    },
  }
</script>