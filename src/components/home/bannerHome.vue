<template>
  <v-app-bar
      app
      color="white"
      flat
      dense

  >

    <img src="../../../public/logoSfn.png" height="80%"/>
    <v-app-bar-title class="bannerHome--title Poppins-Light">
      Instituto Pakal
    </v-app-bar-title>
    <v-spacer/>

    <v-btn
        text
    >
      <span>Inicio</span>
    </v-btn>
    <v-btn
        text
    >
      <span>Galeria</span>
    </v-btn>
  </v-app-bar>
</template>

<script>
export default {
  name: "bannerHome"
}
</script>

<style scoped>

.bannerHome--title{
  margin-left: .5rem;
}

</style>