/* 
Descrizione:
Create un nuovo progetto utilizzando Vue CLI e definite i componenti necessari per strutturare il layout come da screenshot allegato.
Quando la struttura a macroblocchi è pronta, popolate le voci di menu dinamicamente usando i data del componente.
Per oggi diamo priorità alla struttura: quando è tutto bello solido, passiamo al Sass!
 */

<template>
  <div id="app">
    <div class="container">
      <SiteHeader />

    <main class="site_main"></main>
    <!-- /.site_main -->

    <footer class="site_footer"></footer>
    <!-- /.site_footer -->
    </div>
  </div>
</template>

<script>
import SiteHeader from '@/components/HeaderComponent.vue';

export default {
  name: 'App',
  components: {
    SiteHeader
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  /* commons */
  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  img{
    max-width: 100%;
  }

  .container{
    width: 1200px;
    margin: 2rem auto;
  }
}


</style>
