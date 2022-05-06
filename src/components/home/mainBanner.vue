<template>
  <div>
    <div class="mainBanner" id="mainBanner">
      <img src="../../static/logo.png"/>
      <h1 class="Poppins--Bold">INSTITUTO<br/>PAKAL<br/><br/></h1>
    </div>
  </div>
</template>
<script>
export default {
  name: "mainBanner"
}
</script>

<style scoped>

.mainBanner{
  display: grid;
  grid-template-columns: 60% 40%;
  margin-bottom: 2rem;
}

.mainBanner img{
  opacity: .1;
  width: 60vw;
  z-index: 1;
}

h1{
  margin-top: 24rem;
  font-size: 60px;
  color: #343434;
  z-index: 2;
}

@media screen and (max-width: 900px) {
  h1{
    margin-top: 15rem;
    font-size: 45px;
  }
}

@media screen and (max-width: 500px) {
  .mainBanner{
    grid-template-columns: 100%;
  }
  h1{
    margin-top: 1rem;
    margin-left: 1rem;
    font-size: 35px;
  }
  .mainBanner img{
    width: 100vw;
  }
}
</style>
