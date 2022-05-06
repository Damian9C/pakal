<template>
  <div class="contact" id="contact">
    <p class="Poppins--Bold contact--tittle">
      Contacto<br/>
    </p>
    <p class="contact--content Poppins">
      Puedes contactarnos a travez de los siguientes medios<br/><br/>
    </p>
    <div class="contactMedia">

      <div class="contactMedia__links--w">
        <img src="../../static/whatsapp.png" class="contactMedia__links--img"/>
        <div class="contactMedia__links--wp">
          <a class="contactMedia__links--wpLink" href="https://api.whatsapp.com/send?phone=5547938937">
            <div>Whatsapp<br/>
              55-4793-8937
            </div>
          </a>
          <a class="contactMedia__links--wpLink" href="https://api.whatsapp.com/send?phone=5569871518">
            <div>
              Whatsapp<br/>
              55-6987-1518
            </div>
          </a>
        </div>
      </div>

      <div class="contactMedia__Links">
        <a class="contactMedia__links--facebook contactMedia__links--facebookTxt" href="https://www.facebook.com/Instituto.PAKAL.Coacalco">
          <img src="../../static/facebook.png" class="contactMedia__links--img"/>
          <p class="contactMedia__links--facebookTxt">
            Facebook<br/>
            Instituto PAKAL
          </p><br/>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "contact"
}
</script>

<style scoped>

.contact{
  background-color: #E1E1E1;
  padding: 3rem 4rem 4rem;
}

.contact--tittle{
  font-size: 2rem;
  text-align: center;
}

.contact--content{
  text-align: center;
  font-size: 1.4rem;
}

.contactMedia {
  align-items: center;
  text-align: center;
  display: grid;
  grid-template-columns: 50% 50%;
}

.contactMedia__links--img{
  height: 100px;
}

.contactMedia__links--w{
  display: flex;
  align-items: center;
  justify-content: center;
}

.contactMedia__links--wp{
  margin: 0 1rem;
}

.contactMedia__links--wpLink{
  margin: 0 1rem;
  text-decoration: none;
  color: black;
}

.contactMedia__links--facebook{
  display: flex;
  align-items: center;
  justify-content: center;
}

.contactMedia__links--facebookTxt{
  margin: 0 1rem;
  text-decoration: none;
  color: black;
}

@media screen and (max-width: 700px) {
  .contactMedia{
    grid-template-columns: 100%;
  }
}

</style>
