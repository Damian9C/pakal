<template>
  <div>
    <main-banner/>

    <about/>
    <career/>
    <contact/>
    <main-footer/>
  </div>
</template>

<script>
  import BannerHome from "../components/home/bannerHome";
  import MainBanner from "../components/home/mainBanner";
  import About from "../components/home/about";
  import MainFooter from "../components/home/mainFooter";
  import Career from "../components/home/career";
  import Contact from "../components/home/contact";
  export default {
    name: 'Home',
    components: {Contact, Career, MainFooter, About, MainBanner, BannerHome},
  }
</script>

<style>
</style>
