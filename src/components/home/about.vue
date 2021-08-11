<template>
  <div>
    <div class="aboutMain" id="aboutUs">
      <p class="aboutMain--title Poppins--Bold">¿Quienes Somos?</p>
      <p class="aboutMain--content Poppins">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ab amet aperiam assumenda dignissimos eaque facere fuga fugit harum hic illum ipsa nihil, praesentium quam quia quo, unde vel. Labore, non?
      </p>
    </div>

    <div class="aboutDetails Poppins">
      <div class="aboutDetails__mission">
        <h2 class="Poppins--Bold">Mision</h2>
        <p class="aboutDetails--content">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. A blanditiis dolore ducimus eius explicabo, facilis fuga impedit ipsum molestiae nihil nostrum numquam odit perferendis perspiciatis quasi, quos tempore unde voluptatibus?
        </p>
      </div>

      <div class="aboutDetails__view">
        <h2 class="Poppins--Bold">Vision</h2>
        <p class="aboutDetails--content">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad debitis delectus deleniti dignissimos earum id illo itaque nihil, nisi placeat quia quidem rem saepe sapiente, sequi sit temporibus ut vero?
        </p>
      </div>

      <div class="aboutDetails__objective">
        <h2 class="Poppins--Bold">Objetivos</h2>
        <p class="aboutDetails--content">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aperiam commodi consequuntur cumque, delectus deleniti dolor ducimus enim facere id illo incidunt modi molestiae numquam placeat quidem recusandae repellendus repudiandae sint?
        </p>
      </div>
      <img src="../../static/star.png" class="aboutDetails--img"/>

      <img src="../../static/eye.png" class="aboutDetails--img"/>

      <img src="../../static/img.png" class="aboutDetails--img"/>
    </div>
  </div>
</template>

<script>
export default {
  name: "about"
}
</script>

<style scoped>

.aboutMain{
  background-color: #1a91ff;
  color: #f6f6f6;
}

.aboutMain--title{
  font-size: 2.5rem;
  text-align: center;
  padding: 3rem 0 2rem;
}

.aboutMain--content{
  text-align: center;
  padding: 0 15rem 4rem;
  font-size: 2rem;
}

.aboutDetails{
  display: grid;
  grid-template-columns: 33% 33% 33%;
  margin: 4rem 5%;
  text-align: center;
}

.aboutDetails--content{
  padding: 0 1rem 1rem;
}

.aboutDetails--img{
  display: block;
  margin: auto;
  height: 75px;
}

@media screen and (max-width: 950px) {
  .aboutMain--content{
    padding: 0 5rem 4rem;
  }
}

@media screen and (max-width: 500px){
  .aboutMain--title{
    font-size: 2rem;
  }

  .aboutMain--content{
    padding: 0 1rem 3rem;
    font-size: 1.5rem;
  }
}

</style>