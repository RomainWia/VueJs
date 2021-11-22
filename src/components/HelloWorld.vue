<template>
  <h1>Piou</h1>
    <div v-if="seen" id="hide">
      <li v-for="item in items" :key="item.prenom">
      {{ item.prenom }}
    </li>
    </div>

    <div id="app" v-on:click="seen = !seen" class="control">
      <a id="button">Hide WATA</a>
    </div>
  </template>

<script>

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      items: [{prenom: "Prénom 1"},{prenom: "Prénom 2"},{prenom: "Prénom 3"},{prenom: "Prénom 4"},{prenom: "Prénom 5"},],
      isHidden: false,
      seen: true
    };
  },
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

  #button {
    color: white;
    padding-right: 10px ;
    padding-left: 10px ;
    padding-bottom: 5px ;
    padding-top: 5px ;
    background-color: lightblue;
  }
</style>
