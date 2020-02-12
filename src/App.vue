<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <HelloWorld msg="Este é o Hello World" />
    <Oi msg="Este é o Oi" />
    <h2>{{ horas }}</h2>
    <p v-if="horas >= 18">Noite</p>
    <p v-if="horas < 18">Dia</p>
    <Multi :n="numero" />
    <Factorial :n="numero" />
    <Primo :n="numero" />
    <Quadrado :n="numero" />
    <Qubo :n="numero" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Oi from "./components/Oi.vue";
import Multi from "./components/Multi.vue";
import Factorial from "./components/Factorial.vue";
import Primo from "./components/Primo.vue";
import Quadrado from "./components/Quadrado.vue";
import Qubo from "./components/Qubo.vue";

export default {
  name: "app",
  components: {
    HelloWorld,
    Oi,
    Multi,
    Factorial,
    Primo,
    Quadrado,
    Qubo
  },
  data() {
    return {
      horas: new Date().getHours(),
      numero: 5
    };
  },
  methods: {
    /*numero(){
      return 2
    }*/
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.card {
  margin: 0 auto;
  float: none;
  margin-bottom: 10px;
  background-color: violet;
}
.card p {
  font-weight: 600;
}
</style>
