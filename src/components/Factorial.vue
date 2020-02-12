<template>
  <div class="card" style="width: 18rem;">
    <div class="card-body">
      <p class="card-text">Facatorial de {{n}} é {{calcula_factorial(n)}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Factorial",
  props: {
    n: Number
  },
  data() {
    return {
      //n : 5
    };
  },
  methods: {
    calcula_factorial(n) {
      let nHoldar = n;
      let resultado = 1;
      while (nHoldar > 0) {
        resultado *= nHoldar--;
      }
      return resultado;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>