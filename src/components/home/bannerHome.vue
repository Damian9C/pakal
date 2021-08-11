<template>
  <v-app-bar
      app
      color="white"
      flat
      dense
      class="bannerHome"
  >

    <img src="../../../public/logoSfn.png" height="80%"/>
    <v-app-bar-title class="bannerHome--title Poppins-Light">
      Instituto Pakal
    </v-app-bar-title>
    <v-spacer/>

    <div v-for="item in links" :key="item.title">
      <v-btn
          text
          small
          @click="scrollToSection(item.route)"
      >
        <span class="Poppins">{{ item.title }}</span>
      </v-btn>
    </div>
  </v-app-bar>
</template>

<script>
export default {
  name: "bannerHome",
  data: () => ({
    links:[
      {
        title: 'Inicio',
        route: 'mainBanner'
      },
      {
        title: 'Sobre Nosotros',
        route: 'aboutUs'
      },
      {
        title: 'Carreras',
        route: 'career'
      },
      {
        title: 'Contacto',
        route: 'mainBanner'
      },
    ]
  }),
  methods: {

    scrollToSection(elementName) {
      window.scrollTo({
        top: document.getElementById(elementName).offsetTop,
        behavior: 'smooth'
      });
    }
  }
}
</script>

<style scoped>

.bannerHome{
  background-color: #ffffff;
  z-index: 100;
}

.bannerHome--title{
  margin-left: .5rem;
}

</style>