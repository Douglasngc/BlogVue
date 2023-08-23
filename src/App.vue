<template>
  <navbar/>
  <img alt="Vue logo" src="./assets/logo.png">
  <hr><br>
  <First msg="Welcome to Your Vue.js App"/>
<footers/>
</template>

<script>
import footers from './components/footers.vue'
import navbar from './components/navbar.vue'
import First from './components/First.vue'

export default {
  name: 'App',
  components: {
    First,navbar,footers
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
  margin-top: -10px;
  display: flex;
  flex-direction: column;
  
}


</style>
