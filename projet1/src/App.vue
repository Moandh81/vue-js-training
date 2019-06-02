<template>
  <div id="app" class="center-align">
    <HelloWorld msg="Ma première application avec vue js"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  }
}
</script>

