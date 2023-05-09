<template>
    <v-carousel class="carousel"
    v-bind:cycle="true"
    show-arrows="hover"
   hide-delimiter-background
   color="white"
>
        <v-carousel-item 
        class="imgCarousel"
        v-for="item in CarouselText"
          :src="item.img"
          cover
        >
        <div class="imgtext">
          <h2>{{item.titolo}}</h2>
          <p>{{item.autore}} </p>
        </div>
      </v-carousel-item>
      
      </v-carousel>
  </template>
  <style>
  .v-carousel-item
  {
    position:relative;
    height: 100vh;
  }
 
  .imgtext 
  {
    z-index:3;
    color:white;
    font-weight: bold;
   text-shadow: #000000 3px 5px 2px;
    position:absolute;
    top:70%;
    left:0;
    padding-left:30px;
    
    
  }
  .imgtext p
  {
    font-size:20px;
  }
  .imgtext h2
  {
    font-size:90px;
  }
</style>
<script setup>


import { ref } from 'vue';

const CarouselText=[
    {
        titolo:"LOGO",autore:"Gruppo 1 ", img:"../../img/plamontagna.jpg"
    },
    {
        titolo:"INFOGRAFICA",autore:"Gruppo 1", img:"../../img/1294117.png"
    },
    {
        titolo:"FUMETTO",autore:"Gruppo 3",img:"../../img/tappi.jpg"
    },
    
    
    
   
]

</script>