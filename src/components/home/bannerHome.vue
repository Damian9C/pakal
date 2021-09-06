<template>
  <div class="bannerHome">
    <v-navigation-drawer v-model="isActive" temporary app>
      <v-list-item class="mt-2">
        <div class="d-flex flex-column">
          <span class="app-logo-title">
            Instituto Pakal Coacalco
          </span>
        </div>
      </v-list-item>

      <v-list>
        <v-divider />

        <v-list-item v-for="(item, i) of menuLinks" :key="i" link @click="scrollToSection(item.route)">
          <v-list-item-content>
            <v-list-item-title class="app-font-size">
              {{ item.title }}
            </v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar elevation="0" fixed class="app-bar-style" color="white" dense app>
      <img src="../../../public/logoSfn.png" height="80%"/>
      <v-app-bar-title>
        Instituto Pakal
      </v-app-bar-title>
      <v-spacer/>

      <div class="d-none d-md-flex">
        <v-btn
            v-for="(item, j) of menuLinks" :key="j"
            text
            small
            :ripple="false"
            @click="scrollToSection(item.route)"
        >
          {{ item.title }}
        </v-btn>
      </div>

      <div class="d-flex d-md-none">
        <v-btn icon @click="openDrawer">
          <v-icon>
            mdi-menu
          </v-icon>
        </v-btn>
      </div>
    </v-app-bar>
  </div>
</template>

<script>
export default {
  name: "bannerHome",
  data: () => ({
    isActive: null,
    menuLinks: [
      {
        title: 'Inicio',
        route: 'mainBanner',
      },
      {
        title: 'Acerca de',
        route: 'aboutUs',
      },
      {
        title: 'Carreras',
        route: 'career',
      },
    ]
  }),
  methods: {
    openDrawer() {
      this.isActive = true;
    },
    scrollToSection(elementName) {
      window.scrollTo({
        top: document.getElementById(elementName).offsetTop,
        behavior: 'smooth'
      });
      this.isActive = false;
    }
  }
}
</script>

<style scoped>
.bannerHome{
}

.app-bar-content {
  display: flex;
  width: 100%;
  align-items: center;
}
.app-logo-title {
  font-weight: bold;
  font-size: 18px;
}
.app-bar-subhead {
  font-weight: 300;
  font-size: 12px;
  letter-spacing: 0.25em;
}
.app-font-size {
  font-size: 14px;
}
/deep/ .v-toolbar__content {
  padding: 0 !important;
}
</style>