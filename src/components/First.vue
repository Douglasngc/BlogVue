<template>
  <div >
    <p>Olá vue</p>
    <h4>olá me chamo {{ namee }} e trabalho como {{ profisa }}</h4>

   
  </div>
</template>

<script>
export default {
  name: 'FirstT',
  data() {
    return{
      namee:'Ratoera',
      profisa:"Developer"
    }
  }
}
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
</style>
