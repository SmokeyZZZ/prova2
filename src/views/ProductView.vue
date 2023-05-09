<template >
    <div class="ciao"   >
        
        <v-container   class="product-container" >
            
            <v-row align="center" >
                <v-col v-for="ciaos in ciao"  align="center"   >
                    <Prodotto  :title="ciaos.titolo" :authors="ciaos.autore" :imgUrl="ciaos.img" />
                </v-col>
            </v-row>
        </v-container>
      
        
        
    </div>
</template>

<script setup>
import Prodotto from '@/components/Prodotto.vue';

import { ref } from 'vue';

const ciao=[
    {
        titolo:"Logo",autore:"Il logo del progetto!",img:"../../img/logo.png"
    },
    {
        titolo:"Infografica",autore:"Una breve infografica che racconta il mondo della sostenibilità \n, mantenendo il focus sullo spreco della plastica",img:"../../img/1294117.png"
    },
    {
        titolo:"Fumetto",autore:"un fumetto che sfrutta un contesto divertente per fungere da denuncia per quanto riguarda lo spreco della plastica" ,img:"../../img/tappi.jpg"
    },
    
    
    
   
]

</script>

<style >


.ciao
{
    background-color: #81D4FA;
    padding-top: 200px ;
    height: 100vh;
}  
.v-row .v-col 
{
    
    justify-content:center;
}

</style>