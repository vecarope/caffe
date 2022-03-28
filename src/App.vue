<template>
  <nav class="navbar navbar-expand-lg p-md-3 fixed-top">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">
      <router-link to="/"> Cafe Rousted </router-link>
      </a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse"> 
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <router-link to="/about" > Sobre Nosotros </router-link>
        <router-link to="/cultivares"> Nuestros cultivares</router-link>
        <router-link to="/tienda"> Tienda </router-link>
      </ul>
    </div>
  </div> 
</nav> 

<router-view/>


</template>

<script>

export default {

 
  
  
}
</script>

<style>
.navbar{
  width: 100%;
  float: left;
  transition: top 0.3s;
   background-color:rgba(14, 14, 12, 0.8);
  
}
.navbar-nav-scroll {
          overflow:scroll;
          color:black;
          
        }

a{
  margin-left: 20px ;
}
a:link{
  text-decoration: none;
}
a:visited{color:whitesmoke}
a:hover{color:coral}


</style>