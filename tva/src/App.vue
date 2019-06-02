<template>
  <div id="app">
     <div class="row justify-content-center text-center">
      <div class="col-6">
    <img alt="Vue logo" src="./assets/tva-image.png">
    <Tva msg="Calcul de la TVA"/>
      </div>
      </div>

  </div>
</template>

<script>
import Tva from './components/Tva.vue'

export default {
  name: 'app',
  components: {
    Tva
  }
}
</script>

<style>
body {
  padding-top : 2rem ;
}
</style>
