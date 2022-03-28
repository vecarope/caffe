<template>
  <div>
    <div class="jumbotron jumbotron-fluid">
    <div class="container">
    <h1 class="display-2">{{texto}}</h1>
    <p class="lead">{{parrafo}}</p>
     <button @click='accion' class="btn btn-outline-danger">{{boton}}</button>
 </div>
 </div>
  </div>
</template>

<script>

import {ref} from 'vue'

export default {
  components:{
  
  },
  
  props:{
     texto : String ,  
     boton : String , 
     parrafo : String,  
},
methods: {
    accion(){
        this.$emit('accion')
    }
},
     
     
     
  }
 
  

</script>

<style >

.jumbotron {
  display:flex; 
   
  margin:0px 0px 0px 0px;
    background: 
 linear-gradient(
  rgba(34, 10, 250, 0.25), 
  rgba(125, 250, 250, 0.45)
), 
;
background-image: url('@/assets/img/grano1.jpg'); 
background-size: cover;
background-repeat: no-repeat;
background-attachment: fixed;
background-position: center;
color:white !important;
height:500px;


}
.container{
  margin-left: 50px;
}
h1{
   padding-top: 70px;
   color:brown; 
   font-weight: 300 , bold;
   
}
button{
  float:left; 
  

}
</style>