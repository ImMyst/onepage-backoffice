<template>
  <v-toolbar color="red lighten-1" max-height="65" class="fixed mx-3">
    <v-toolbar-title class="headline">
      Titouan GALVANI
    </v-toolbar-title>
    <v-spacer />
    <div class="px-3">
      <v-btn text href="#about">A propos</v-btn>
      <v-btn text href="#projects">Projets</v-btn>
      <v-btn text href="#skills">Compétences</v-btn>
      <v-btn text href="#contact">Contact</v-btn>
    </div>
    <v-spacer />
    <v-toolbar-items>
      <v-btn text>Login</v-btn>
    </v-toolbar-items>
  </v-toolbar>
</template>

<style lang="sass" scoped>
.fixed
  position: fixed
  width: 100%
  z-index: 99
</style>
