<template>
  <div>
    <main-banner/>
  </div>
</template>

<script>
  import BannerHome from "../components/home/bannerHome";
  import MainBanner from "../components/home/mainBanner";
  export default {
    name: 'Home',
    components: {MainBanner, BannerHome},
  }
</script>

<style>
</style>
