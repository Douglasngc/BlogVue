<template>
  
  <ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
  <div class="dropdown" style="float:right;">
  <button class="dropbtn">Login</button>
  <div class="dropdown-content">
  <a href="#">Entrar</a>
  
  </div>
</div>
</ul>
</template>

<script>
export default {
    name: 'navbarR'

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
.test{
    text-color:white;
    
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