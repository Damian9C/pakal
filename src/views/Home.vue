<template>
  <div>
    <main-banner/>

    <about/>


    <main-footer/>
  </div>
</template>

<script>
  import BannerHome from "../components/home/bannerHome";
  import MainBanner from "../components/home/mainBanner";
  import About from "../components/home/about";
  import MainFooter from "../components/home/mainFooter";
  export default {
    name: 'Home',
    components: {MainFooter, About, MainBanner, BannerHome},
  }
</script>

<style>
</style>
