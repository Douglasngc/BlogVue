<template>
  
  <ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
  <div v-if="isLogged" key="sucesss">
  <button v-on:click.prevent="toggleLogin" style="float:right;" class="dropbtn">Fazer logout</button>
  </div>

<button v-on:click.prevent="toggleLogin" style="float:right;" class="dropbtn" v-else key="error">Fazer login</button>
</ul>
</template>

<script>
export default {
    name: 'navbarR',
  data() {
    return{
      
      isLogged: false,
      nome: 'dg'
    }
  },
  methods:{
    toggleLogin(){
      this.isLogged = !this.isLogged;
    }

  }
  }


</script>

<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

li {
  float: left;
}

li a, .dropbtn {
  display: inline-block;
  color: rgb(228, 97, 9);
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}
.dropbtn{
    background: #333;
}

li a:hover, .dropdown:hover .dropbtn {
  background-color: rgb(0, 0, 0);
}

li.dropdown {
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #333;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px #333;
  z-index: 1;
  
}

.dropdown-content a {
    color: rgb(228, 97, 9);
  padding: 12px 16px;
  text-decoration: none;
  display: block;
  text-align: left;
}

.dropdown-content a:hover {background-color: #000000;}

.dropdown:hover .dropdown-content {
  display: block;
}
</style>