<template>
  <div class="aboutUs">
    <p>
      Tato stránka vám v jednoduchých krocích pomůže naplánovat trasu a vytvořit
      vlastní itinerář cesty do vybraného místa v České republice.
      <br>
      Jako uživatel
      si nejprve vyberte cílovou destinaci, kam chcete jet. K tomu může
      posloužit <router-link to="/places/all">přehled měst</router-link> v menu v hlavičce stránky. Když už
      víte kam zamíří vaše kroky, naplánujte si vlastní itinerář <router-link to="/itinerary">zde.</router-link> Do formuláře pak už jen stačí zakliknout body - místa, která
      chcete navštívit a následně se trasa vykreslí a přehledně zobrazí na mapě. Využijte i další tlačítka, díky nim si můžete výlet naplánovat pěšky, autem, či využijete městskou hromadnou dopravu.
    </p>

<img class="img-menu case" :src="`./assets/img/bgr-img (1).png`" />

<img class="img-menu van" :src="`./assets/img/bgr-img (2).png`" />
   

    <img class="img-menu alp" :src="`./assets/img/bgr-img (4).png`" />
    <img class="img-menu gyro" :src="`./assets/img/bgr-img (6).png`" />
  </div>
</template>

<script>
export default {
  name: "AboutUs"
};
</script>

<style>
html {
  background-color: rgb(254, 250, 242);
}

p a {
text-decoration: underline;
  color: #EC7568;
  font-weight: bold;
}

.van {
    right: 43vw;
    position: absolute;
    top: 82vh;
    
}

.aboutUs {
  background-color: rgb(254, 250, 242);
  min-height: 100vh;
}

.aboutUs p {
  position: relative;
  text-align: justify;
  padding: 30px;
  margin: 130px 40px 0 40px;
  background-color: #bcdde2;
  border-radius: 20px;
  box-shadow: 22px 23px 29px -9px rgba(0, 0, 0, 0.67);
  color: rgba(0, 0, 0, 1.67) !important;
  font-size: 1.2em;
}

.van {
     right: 180px;
    position: absolute;
    top: 500px;
}

.alp {
     right: 450px;
    position: absolute;
    top: 150px;
  
}

.case {
      left: 100px;
    position: absolute;
    top: 550px;
}
.gyro {
  right: 10px;
    position: absolute;
    top: 100px;
}



@media screen and (max-width: 860px) {
  .case, .van, .alp, .gyro {
    display: none;
  }
}





</style>
