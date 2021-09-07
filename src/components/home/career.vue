<template>
  <div>
    <div class="career" id="career">
      <p class="career--tittle Poppins--Bold">Licenciaturas</p>
      <p class="career--subTittle Poppins">
        Contamos con Licenciatuaras en 9 cuatrimestres<br/><br/><br/>

        <img src="../../static/licenciated.png" class="career--img"/>
      </p><br/>
    </div>

    <div class="careersDescription">
      <div class="careersDescription--pedagogy">
        <p class="careersDescription--title Poppins--Bold">Pedagogía</p><br/>
        <p class="careersDescription--txt Poppins">
          La Licenciatura en Pedagogía que se imparte en esta institución, tiene como objetivo principal el formar profesionales que cuenten con los conocimientos necesarios para comprender y afrontar el contexto educativo actual de nuestro país, así como aplicar los mecanismos que los procesos sociales, económicos, políticos y culturales exigen de los distintos niveles de la educación.
        </p><br/>

        <img src="../../static/pedagogy.png" class="careersDescription--img"/><br/><br/><br/>
      </div>

      <v-divider/>
      <br/>
      <br/>

      <div class="careersDescription--admon">
        <p class="careersDescription--title Poppins--Bold">Administración<br/>de Empresas</p><br/>
        <p class="careersDescription--txt Poppins">
          La Licenciatura en Administración de Empresas que se imparte en esta institución, tiene como principal objetivo, formar profesionales con la capacidad suficiente para implementar mecanismos eficaces y soluciones para las necesidades de la empresa fomentando así el crecimiento de la misma. Los egresados de esta carrera obtienen una metodología para aprender a resolver problemas en situaciones cambiantes y adquieren un criterio profesional para poder discernir sobre diversas actividades.
        </p><br/>

        <img src="../../static/admon.png" class="careersDescription--img"/>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "career"
}
</script>

<style scoped>

.career{
  background-color: #e1e1e1;
  text-align: center;
}

.career--tittle{
  font-size: 2rem;
  text-align: center;
  padding: 3rem 0 2rem;
}

.career--subTittle{
  font-size: 1.4rem;
}

.career--img{
  display: block;
  margin: auto;
  height: 100px;
}

.careersDescription{
  text-align: center;
  margin: 3rem 8rem 8rem;
}

.careersDescription--title{
  font-size: 2rem;
}

.careersDescription--txt{
  font-size: 1.4rem;
}

.careersDescription--img{
  display: block;
  margin: auto;
  height: 200px;
}

@media screen and (max-width: 900px) {
  .careersDescription{
    margin: 3rem 2rem 8rem;
  }
}

@media screen and (max-width: 500px) {
  .career--subTittle{
    padding: 0 1rem;
  }
}

</style>