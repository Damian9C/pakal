<template>
  <div>
    <div class="mainBanner">
      <v-spacer/>

      <v-spacer/>
    </div>
    <h1 class="Poppins--Bold">INSTITUTO<br/>PAKAL</h1>
    TEXTO AL AZAR
  </div>
</template>
<script>
export default {
  name: "mainBanner"
}
</script>

<style scoped>

.mainBanner {
  position: absolute;
  overflow: hidden;
  padding: 16px;
  background-image: url("../../static/logo.png");
  background-size: 40em;
  background-repeat: no-repeat;
  filter: opacity(40%);
  width: 100vw;
  height: 100vh;
  z-index: 100;
}

h1 {
  padding: 10rem 8rem 15rem 40rem;
  font-size: 64px;
  color: #343434;
  z-index: 1;
}
</style>