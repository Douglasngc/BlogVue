<template>
  <navbar/>
  <img alt="Vue logo" src="./assets/logo.png">
  <hr><br>
  <First msg="Welcome to Your Vue.js App"/>
</template>

<script>
import navbar from './components/navbar.vue'
import First from './components/First.vue'

export default {
  name: 'App',
  components: {
    First,navbar
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
  display:block ;
 
}


</style>
