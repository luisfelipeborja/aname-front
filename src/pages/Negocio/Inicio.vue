<template>
  <!--Carrusel-->


  <div id="carousel1" class="carousel slide" data-bs-ride="carousel">
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="@/assets/img/img-slide-01.jpg" class="d-block w-100" alt="">
      </div>
      <div class="carousel-caption d-none d-md-block">
        <h1 style="color: #ffffff; text-align:left; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.8);">
          ASOCIACIÓN NACIONAL DE ATLETISMO MÁSTER</h1>
      </div>
      <div class="carousel-item">
        <img src="@/assets/img/img-slide-02.jpg" class="d-block w-100" alt="">
      </div>
      <div class="carousel-caption d-none d-md-block">
        <h1 style="color: #ffffff; text-align:left; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.8);">
          ASOCIACIÓN NACIONAL DE ATLETISMO MÁSTER</h1>
      </div>
      <div class="carousel-item">
        <img src="@/assets/img/img-slide-03.jpg" class="d-block w-100" alt="">
      </div>
      <div class="carousel-caption d-none d-md-block">
        <h1 style="color: #ffffff; text-align:left; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.8);">
          ASOCIACIÓN NACIONAL DE ATLETISMO MÁSTER</h1>
      </div>
      <div class="carousel-item">
        <img src="@/assets/img/img-slide-04.jpg" class="d-block w-100" alt="">
      </div>
      <div class="carousel-caption d-none d-md-block">
        <h1 style="color: #ffffff; text-align:left; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.8);">
          ASOCIACIÓN NACIONAL DE ATLETISMO MÁSTER</h1>
      </div>
      <div class="carousel-item">
        <img src="@/assets/img/img-slide-05.jpg" class="d-block w-100" alt="">
      </div>
      <div class="carousel-caption d-none d-md-block">
        <h1 style="color: #ffffff; text-align:left; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.8);">
          ASOCIACIÓN NACIONAL DE ATLETISMO MÁSTER</h1>
      </div>
    </div>
    <!--botón anterior-->
    <button class="carousel-control-prev" type="button" data-bs-target="#carousel1" data-bs-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Anterior</span>
    </button>
    <!--botón siguiente-->
    <button class="carousel-control-next" type="button" data-bs-target="#carousel1" data-bs-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Siguiente</span>
    </button>
  </div>


  <!--Barra navegacion-->
  <div v-if="mostrarBarra">
    <BarraNav />
  </div>
  <div v-else>
    <BarraNavPro />
  </div>
  <div class="page-content">
    <!-- Contenido -->
    <main>
      <div class="container" id="contenido">
        <div class="col" id="banner">
          <img class="img-fluid mx-auto d-block" alt="Banner Principal" src="@/assets/img/bannerprincipal.png">
        </div>

        <div class="card mb-2" id="cardPersonalizada">
          <div class="row g-4">
            <div class="col-md-6">
              <img src="@/assets/img/card_a.png" class="img-fluid rounded-start" alt="...">
            </div>
            <div class="col-md-6 d-flex align-items-center">
              <div class="card-body">
                <h5 class="card-title fs-2 fw-bold text-center" id="textCard1">ANAME como parte del Sistema Deportivo
                  Nacional
                </h5>
                <p class="card-text" id="textCard1">El atletismo máster acoge a deportistas desde los 30 años en adelante,
                  divididos en modalidades de acuerdo a las edades de los participantes.
                  En Ecuador la organización promotora de estas competencias es la Asociación Nacional de Atletas Master
                  del Ecuador (ANAME).</p>
                <p class="card-text" id="textCard2"><small>La ANAME fue fundada el 18 de septiembre de 2011.</small></p>
              </div>
            </div>
          </div>
        </div>

        <div class="container-fluid" id="infoRelacionada">
          <div>
            <h2 class="text-center text-uppercase" id="textTitleInfo">Información Relacionada</h2>
          </div>
          <div class="row">
            <div class="col" style="border-right: 4px solid #52bad1;">
              <a href="https://asudama.org/"><img src="@/assets/img/logo-asudama.png" class="imgAsudama"></a>
            </div>
            <div class="col" style="padding-top: 10px;">
              <div class="card" style="display: flex; justify-content: space-between; align-items: center;">
                <div class="card-body">
                  <h5 class="card-title fw-bold">2024 SOUTH AMERICAN COMBINED EVENTS CHAMPIONSHIPS</h5>
                  <p class="card-text">Sede: Mar de Plata, Argentina</p>
                  <a href="https://asudama.org/" class="card-link" style="color: #2660a4;">Más información</a>
                </div>
              </div>
            </div>
          </div>
          <hr>
          <div class="row">
            <div class="col" style="border-right: 4px solid #52bad1;">
              <a href="https://world-masters-athletics.org/championships/2024-european-championships-indoor/"><img
                  src="@/assets/img/ema-logo.png" class="imgWma"></a>
            </div>
            <div class="col" style="padding-top: 10px;">
              <div class="card" style="display: flex; justify-content: space-between; align-items: center;">
                <div class="card-body">
                  <h5 class="card-title fw-bold">2024 EUROPEAN CHAMPIONSHIPS INDOOR</h5>
                  <p class="card-text">Sede: Torún, Polonia</p>
                  <a href="https://world-masters-athletics.org/championships/2024-european-championships-indoor/"
                    class="card-link" style="color: #2660a4;">Más información</a>
                </div>
              </div>
            </div>
          </div>
        </div>

      </div>
      <p class="textFoot">Este proyecto fue desarrollado para poner en práctica los conocimientos
        adquiridos en la materia de Computación Grid y Cloud, por los estudiantes de las carreras de Ingeniería en
        Computación e Ingeniería en Computación Gráfica de la Universidad Central del Ecuador.</p>
    </main>
  </div>
  <!-- Pie de página -->
  <PiePagina />
</template>

<script>
import PiePagina from '@/components/PiePagina.vue'
import BarraNav from '@/components/BarraNav.vue'
import BarraNavPro from "@/components/BarraNavPro.vue";

export default {
  name: 'Inicio',
  components: {
    BarraNavPro,
    PiePagina,
    BarraNav,
  },
  mounted() {
    console.log("listo NicoMachin sisisisisisis");
    console.log("ROL INICIO" + sessionStorage.getItem("rol"))
    if (sessionStorage.getItem("rol") == "ADM" || sessionStorage.getItem("rol") == "JUN" || sessionStorage.getItem("rol") == "ORG") {
      console.log("id: " + sessionStorage.getItem("id"))
      this.mostrarBarra = false;
    }
  },
  data() {
    return {
      mostrarBarra: true
    }
  }
}

</script>

<style scoped>
.carousel-item {
  max-height: 348px;
  /* Ajusta la altura */
}

.carousel-item img {
  width: auto;
  height: auto;
}

#banner {
  padding-bottom: 40px;
  margin-bottom: 40px;
  border-bottom: 4px solid #52bad1;
}

#cardPersonalizada {
  padding-bottom: 20px;
  padding-top: 20px;
  padding-left: 20px;
  padding-right: 20px;
  background-color: #52bad1;
}

#textCard1 {
  color: black;
}

#textCard2 {
  color: #edf3f5;
}

#textTitleInfo {
  margin-top: 50px;
}

.textFoot {
  margin-top: 20px;
  margin-left: 8%;
  margin-right: 8%;
  margin-bottom: 20%;
}

.imgWma {
  width: 170px;
  height: auto;
  margin-top: 30px;
}

.imgAsudama {
  height: 150px;
}

#infoRelacionada {
  padding-bottom: 15px;
}

#contenido {
  background-color: #edf3f5;
  padding-bottom: 30px;
  padding-top: 30px;
  padding-left: 120px;
  padding-right: 120px;
}

@media (min-width: 320px) {
  #contenido {
    padding-left: 15px;
    padding-right: 15px;
  }
}

.page-content {
  padding-bottom: 20%;
}
</style>
