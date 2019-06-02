<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p> C'est ici que je vais m'amuser</p>
    <a class="waves-effect waves-light btn " @click="ajouter()" :class="{disabled : max}"> On appuie ici</a>
    <p>On va compter un peu : {{ compteur}}</p>
   


  <div v-if="max" class="row">
    <div class="col s4 offset-s4">
      
          <div class="card-panel red"><span class="white-text">Vous avez atteint le maximum !</span></div>


    </div>
  </div>

  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data : function() {
    return {
      compteur : 0,
      max : false
    }
  },
  methods : {


    ajouter() {
       if (this.compteur < 10) {
        this.compteur ++
       }

       else {
        this.max = true
       }
    }


  },

  props : {
    msg : String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
