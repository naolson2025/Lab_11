<template>
  <div id="app">
    <!--Anything between the HelloWorld tags can be rendered from a slot in HelloWorld.vue-->
    <HelloWorld msg="Welcome to Your Vue.js App">
      <!--This text "Hello, Students" will be passed to the HelloWorld component and rendered in a slot-->
      <img src="./assets/icons8-hello-24.png">
      <p>Hello, Students</p>
    </HelloWorld>
  </div>
</template>

<script>
  // import HelloWorld as child component
import HelloWorld from './components/HelloWorld.vue'
  // import HelloNamed as child component
import HelloNamed from './components/HelloNamed'

export default {
  name: 'app',
  components: {
    HelloWorld, HelloNamed
  }
}
</script>

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
