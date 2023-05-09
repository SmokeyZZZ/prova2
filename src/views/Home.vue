<template>
  <div class="homeView">
      
      
        <Carousel height="95vh"/>

        <v-row class="content"  >
            <!--<v-col class="slogan">
                <h1>LIFE IN </h1><h1><span class="highlighted">PLASTIC</span></h1>
                <h1>ISN'T </h1><h1><span class="highlighted"> FANTASTIC</span></h1>
            </v-col>-->
            <v-col class="slogan">
                <h1>Il nostro obiettivo è <span class="highlighted">promuovere il cambiamento</span>, per un mondo migliore!</h1>
           
            <v-btn class="more" color="#B3E5FC"><router-link to="/project">di più sul progetto</router-link></v-btn></v-col>
        </v-row>
    
  </div>
  </template>
  <style>
  @font-face {
    font-family: space-grotesk;
    src: url(font/space-grotesk-2.0.0/fonts/otf/SpaceGrotesk-Bold.otf);
  }
  .content{background-color: inherit;}
.homeView{background-color:#81D4FA;height: 100%;}
.content
{  
    height:100vh;
    display:flex;
    padding:50px;

    align-items: center;
    
}

.slogan
{
    color: blue;
    
    z-index: 3;
    font-size: 50px;
    text-shadow: #000000 3px 3px 3px;
    text-align: center;
    text-transform: uppercase;
}
.more{float:center; font-size:20px; color:black;}

.highlighted
{
    color:aqua;
}
  *{list-style-type: none;}
</style>
  <script setup >
  import Carousel from '../components/Carousel.vue';
  import Prodotto from '../components/Prodotto.vue';
  </script>
  
  
  