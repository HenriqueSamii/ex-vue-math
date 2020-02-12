<template>
  <div class="card" style="width: 18rem;">
    <div class="card-body">
      <p class="card-text">Quadrado de {{n}} é {{quadrado(n)}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Quadrado",
  props: {
    n: Number
  },
  data() {
    return {
      //n : 5
    };
  },
  methods: {
    quadrado(n) {
      return n ** 2;
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