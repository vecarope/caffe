<template>
<div class="container">
<div class="row row-cols-4 row-cols-md-3 g-5">
<div class="col" v-for="(cafe, index) of cafes" :key="index">
    <div class="card">
    <img :src='cafe.Img' class="card-img-top" :alt="`imagen-${cafe.Nombre}`">
    <div class="card-body">
        <h4 class="card-title">{{cafe.Nombre}}</h4>
        <p class="card-text">Variedad:{{cafe.Variedad}}</p>
        <router-link :to="{ name:'Producto', params:{id:index}}">
    <button class="btn btn-outline-danger"> conocer mas... </button>
        </router-link>
    </div>
    </div>
</div>  
    </div>
    </div>
</template>

<script>
import {mapState} from 'vuex'
export default {

    computed:{
        ...mapState (['cafes'])
    },
}
</script>

<style>
.container{
    width: 100%;
    height:100%;
    justify-content: center;
    flex-wrap: wrap;
    display: flexbox, 
    


}
.col{
    width: 380px;
}
.card{
    text-align: center;
    font-size: 40px;
    color: #6a6a6a;
    margin-top: 100px;
    font-weight: 100;
    font-family: 'Roboto', sans-serif;
}
.container .card{
    width: 330px;
    height: 430px;
    border-radius: 8px;
    box-shadow: 0 2px 2px rgba(0, 0, 0, 0.2);
    overflow: hidden;
    margin: 20px;
    text-align: center;
    transition: all 0.25s;

}
.container .card img{
    width: 330px;
    height: 220px;
}
.container .card h4{
    font-weight: 600;
}

.container .card p{
    padding: 0 0rem;
    font-size: 16px;
    font-weight: 300;
}

.container .card a button{
    font-weight: 500;
    text-decoration: none;
    color: #3498db;
    
}

.container .card:hover{
    transform: translateY(-15px);
    box-shadow: 0 12px 16px rgba(0, 0, 0, 0.2);
}
button{
    float:none; 
}


</style>