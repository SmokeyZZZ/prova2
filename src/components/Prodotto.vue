<template>
   <a href=""><v-card
   class="carta"
    width="450"
    max-width="450"
    color="#B3E5FC"
  >
    <v-img
    :src="imgUrl"
      height="350px"
      cover
    ></v-img>

    <v-card-title class="title">
     {{ title }}
    </v-card-title>

    <v-card-subtitle class="subtitle">
      {{ authors }}
    </v-card-subtitle>
  </v-card>
  </a>
</template>

<script setup >
const props = defineProps({
  title: String,
  authors:String,
  imgUrl:String,
})

</script>

<style scoped>
.title{font-size:30px;}
.carta{
  text-align:center;
}
.subtitle
{
  padding:10px 0;
}
</style>