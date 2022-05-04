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
@import '~@/assets/scss/style.scss';
</style>
