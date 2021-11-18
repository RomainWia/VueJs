<template> <!-- template DOM -->
  <img alt="Vue logo" src="./assets/logo.png"> <!-- img classique -->
  <HelloWorld msg="Welcome to Your Vue.js App"/> <!-- composant car la balise possède une majuscule -->
</template>

<script> // Javascript
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style> /* CSS */
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
