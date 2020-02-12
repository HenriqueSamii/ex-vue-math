<template>
  <div class="card" style="width: 18rem;">
    <div class="card-body">
      <p class="card-text">{{n}}{{primo(n)}}é Primo</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "primo",
  props: {
    n: Number
  },
  data() {
    return {
      //n : 5
    };
  },
  methods: {
    primo(n) {
      for (let i = n - 1; i > 1; i--) {
        if (n % i == 0) {
          return " não ";
        }
      }
      return " ";
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