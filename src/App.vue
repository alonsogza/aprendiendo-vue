<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <!-- Este es "MiComponente.vue" pero para usarlo se requiere IMPORTARLO, en caso contrario no lo reconoce -->
  <MiComponente></MiComponente> 
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import MiComponente from './components/MiComponente.vue' // Aqui se IMPORTA


export default {
  name: 'App',
  components: {
    HelloWorld,
    MiComponente // En esta parte ya lo reconoce el App.vue
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
