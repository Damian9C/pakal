<template>
  <div>
    <main-banner/>

    <about/>
    <career/>
    <main-footer/>
  </div>
</template>

<script>
  import BannerHome from "../components/home/bannerHome";
  import MainBanner from "../components/home/mainBanner";
  import About from "../components/home/about";
  import MainFooter from "../components/home/mainFooter";
  import Career from "../components/home/career";
  export default {
    name: 'Home',
    components: {Career, MainFooter, About, MainBanner, BannerHome},
  }
</script>

<style>
</style>
