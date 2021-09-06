<template>
  <div>
    <div class="aboutMain" id="aboutUs">
      <p class="aboutMain--title Poppins--Bold">¿Quienes Somos?</p>
      <p class="aboutMain--content Poppins">
        Somos un grupo de profesionistas entusiastas dedicados y comprometidos con la educación mexicana, nos hemos reunido para formar una Institución donde se encuentren presente los valores que se han perdido en México, el amor, el trabajo y conocimiento, así como la lealtad y la honradez.
      </p>
    </div>

    <div class="aboutDetails Poppins">
      <div class="aboutDetails__mission">
        <img src="../../static/star.png" class="aboutDetails--img"/><br/>
        <h2 class="Poppins--Bold">Mision</h2><br/>
        <p class="aboutDetails--content">
          Formar personas íntegras, con una visión humanística y competitiva en su campo profesional, que persigan la búsqueda de una cultura propia y un servicio profesional para todo su entorno.
        </p>
      </div>

      <div class="aboutDetails__view">
        <img src="../../static/eye.png" class="aboutDetails--img"/><br/>
        <h2 class="Poppins--Bold">Vision</h2><br/>
        <p class="aboutDetails--content">
          Para el año 2021 debemos ser la institución educativa más reconocida en la zona por sus egresados, quienes promoverán la competitividad a través de modelos y sistemas para el desarrollo de su comunidad.
        </p>
      </div>

      <div class="aboutDetails__objective">
        <img src="../../static/img.png" class="aboutDetails--img"/><br/>
        <h2 class="Poppins--Bold">Valores</h2><br/>
        <p class="aboutDetails--content">
          OJEL - Amor<br/>
          JAAJIL - Trabajo<br/>
          YAJ - Conocimiento<br/>
          KAXÁANT - Lealtad, Honradez
        </p>
      </div>


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

@media screen and (max-width: 700px){
  .aboutDetails{
    grid-template-columns: 100%;
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