<script>
  import HelloWorld from './components/HelloWorld'
  import Profesores from './components/Profesores'

  export default {
    name: 'App',
    components: {
      HelloWorld, Profesores
    }
  }
</script>

<template>
  <div id="app">
    <div class="container">
      <img src="./assets/logo.png">
      <HelloWorld/>
      <Profesores/>
    </div>
  </div>
</template>


<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
