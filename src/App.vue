<template>
  <div id="app">
    <!-- <img src="./assets/logo.png"> -->
    <HelloWorld msg="Welcome to Your Vue.js App, fol the wol"/>
    <Directives message="This is another components"></Directives>
    <DataBinding></DataBinding>
  </div>
</template>

<script>
  import HelloWorld from './components/HelloWorld.vue'
  import DataBinding from './components/DataBinding.vue'
  import Directives from './components/DataBinding.vue'

  export default {
    name: 'app',
    components: {
      HelloWorld,
      DataBinding,
      Directives
    }
  }
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    /* color: #2c3e50; */
    margin-top: 60px;
  }
</style>
