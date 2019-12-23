
<template>
  <q-layout view="hHh lpR fFf">
    <q-header elevated class="flat text-white flex" height-hint="112" q-p-none>
      <q-tabs align="left ">
        <q-route-tab to="#" label="Oposición Bomberos" />
      </q-tabs>
        <q-space />
      <q-tabs>
        <q-route-tab to="/page1" label="Precios" />
        <q-route-tab to="/page2" label="Login / Signin" />
      </q-tabs>
    </q-header>
      <q-banner class="hero-banner">
        <div class="banner-text">
          <h1>Conviértete en Bombero</h1>
          <p class="subtitle">
            La mayor Base de Datos de preguntas de examen
          </p>
          <q-btn class="btn-big" size="lg"  color="red" label="Prueba Gratis" />
        </div>
      </q-banner>
      <div class="quotes">
        <h1>2.000+ Preguntas de Examen</h1>
        <p>con las que prepararte para aprobar la Oposicion de Bombero</p>
      </div>
      <NewsCarousel/>
    <q-footer elevated class="bg-grey-8 text-white">
      <q-toolbar>
        <q-toolbar-title>
        </q-toolbar-title>
      </q-toolbar>
    </q-footer>
  </q-layout>
</template>

<script>
import NewsCarousel from '../components/NewsCarousel.vue'
export default {
  data () {
    return {}
  },
  components: {
    NewsCarousel
  }
}
</script>
<style lang="scss" scoped>
.nav-bar {
  background-color: rgba(184, 0, 0, 1);
}
.hero-banner {
  background-image: url('../statics/assets/banner.jpg');
  height: 100vh;
  background-position: center;
  background-size: cover;
  background-blend-mode: darken;
}
.banner-text {
  text-align: right;
  margin-right: 10%;
  h1 {
    color: #ffffff;
    font-size: 3.6rem;
    margin-bottom: 20px;
    line-height: unset;
    z-index: 1;
    font-family: 'Roboto Condensed', sans-serif;
    font-weight: 700
  }
  p {
    color: #ffffff;
    font-size: 1.65rem;
    margin-top: 0px;
    line-height: unset;
    font-family: 'Roboto Condensed', sans-serif;
    font-weight: 300;
    z-index: 1;
  }
}
.btn-big {
  font-family: 'Roboto Condensed', sans-serif;
  font-weight: 400;
}
.quotes {
  height: 400px;
  text-align: center;
  padding-top: 7rem;
  h1 {
    font-size: 3.4rem;
    color: #da3e3e;
  }
  p {
    font-size: 1.7rem;
  }
}
//table
.table-wraper {
  margin: 0 auto;
  background-image: url('../statics/assets/table.jpg');
  background-size: cover;
  background-position: center;
  height: 550px;
  width: 100%;
  padding-top: 1rem;
}
.table-container {
  width: 70%;
  margin: 0 auto;
}
.columns {
  float: left;
  width: 33.3%;
  padding: 8px;
}
.price {
  list-style-type: none;
  margin: 0;
  padding: 0;
  -webkit-transition: 0.3s;
  transition: 0.3s;
}
.price .header {
  background-color: #da3e3e;
  color: white;
  font-size: 25px;
}
.price li {
  padding: 20px;
  text-align: center;
  background-color: white;
}
.button {
  background-color: rgb(0, 129, 204);
  border: none;
  color: white;
  padding: 10px 25px;
  text-align: center;
  text-decoration: none;
  font-size: 18px;
}
.v-footer {
  background-color: #da3e3e;
}

.subtitle {
  line-height: 40px;
}
</style>
