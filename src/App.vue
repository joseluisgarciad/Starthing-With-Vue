<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <StartingWithVue msg="Welcome ro your starter component" class="border border-success"/><hr>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'
import StartingWithVue from './components/StartingWithVue.vue'


export default {
  name: 'App',
  components: {
    HelloWorld,
    StartingWithVue,
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
