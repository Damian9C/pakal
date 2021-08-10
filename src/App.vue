<template>
  <v-app>
    <banner-home/>
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

import BannerHome from "./components/home/bannerHome";
export default {
  name: 'App',
  components: {BannerHome},
  data: () => ({
    //
  }),
};
</script>

<style>

</style>