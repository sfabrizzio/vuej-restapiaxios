<template>

<v-layout row wrap align-center>
    <v-flex XS9 offset-md2>
   <div v-for="article in articles" :key="article.title">
  <v-card class="my-3" hover>
<v-img height="350px"  max-width="1080" v-bind:src="article.urlToImage">

</v-img>
  </v-card>
   </div>
    </v-flex>
</v-layout>
</template>
<script>


export default ({
   name:"main-content",
   props : {
       articles :Array
   }
})
</script>
