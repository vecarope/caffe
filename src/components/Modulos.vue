<template>
<div class="card bg-dark text-white">
  <img src="" class="card-img" alt="">
  <div class="card-img-overlay">
    <h5 class="card-title">{{tituloModulo}}</h5>
    <p class="card-text">{{textoModulo}}</p>
  </div>
  
</div>
</template>

<script>

export default {

    props: {
        tituloModulo : String, 
        textoModulo : String, 
    },
 

}
</script>
 

<style scoped>
div{
  margin-left: 0;
}
.card{
    margin: 100px 0px 0px 0px ;
    width: 99%;
    height:400px ;
    justify-content: center;
    display: flex;
}

 h5{
padding-top: 70px;
   color:brown; 
   font-weight: 600 , bold;
 }
</style>