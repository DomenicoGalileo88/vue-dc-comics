/* 
Descrizione:
Create un nuovo progetto utilizzando Vue CLI e definite i componenti necessari per strutturare il layout come da screenshot allegato.
Quando la struttura a macroblocchi è pronta, popolate le voci di menu dinamicamente usando i data del componente.
Per oggi diamo priorità alla struttura: quando è tutto bello solido, passiamo al Sass!
 */

<template>
  <div id="app">
    
    <SiteHeader />

    <SiteMain />

    <SiteFooter />

  </div>

</template>

<script>
import SiteHeader from '@/components/HeaderComponent.vue';
import SiteMain from '@/components/MainComponent.vue';
import SiteFooter from '@/components/FooterComponent.vue';

export default {
  name: 'App',
  components: {
    SiteHeader,
    SiteMain,
    SiteFooter,
  }
}
</script>

<style lang="scss">
 /* commons */
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }


#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  .wrapper{
    width: 1200px;
    margin: 2rem auto;
  }
}

</style>
